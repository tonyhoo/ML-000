### Python 性能优化
#### 识别代码瓶颈 - profiler
* cProfile
* line_profiler
* VTune (推荐,收费，学生免费)
* 寻找原因
    * 不论是CPU/GPU, 内存读取往往是核心
        * 内存层次：内存 -> Cache -> Register
        * 理解
            * 内存： 仓库；汽车 能程序控制
            * Cache： 货架； 飞机
                * 一般来说内存地址是成批进Cache的
                * 如果不在一块儿就非常麻烦，example: row based stored matrix with column operation
                * Branch Prediction， CPU一般会提前判断if else branch的执行来cache，所以通用的代码放在if 里面
                * 多线程改一段内存，由于内存一定要和cache一致，导致读取很多
                * [VTune cookbook](https://software.intel.com/content/www/us/en/develop/documentation/vtune-cookbook/top.html)
                * 方法
                    * paragma
                    * cache-miss-rate来看命中率
            * Register: 工作台; 火箭 但不能控制
    * SIMD是提速非常好的方法
        * 现代CPU往往可以同时进行多个运算(register 更大)，但是操作必须是一样的（比如说加或者乘）
        * 实现方式
            * OpenMP 指令 （只能用C/C++）
            * 需要directory
            * 或者使用intrinsics（近乎汇编）
* 找到瓶颈后
    * 换框架 mySQL -> Reddis
    * 改代码 
#### 宏观上寻找修改
#### 采用Cython 或者C++
* [官网](https://cython.org)
* Python superset，全部Python代码都能跑
* 更好的方法是想象成C
* 最大区别，静态类速度快，不需要去做type inference然后看operator重载
* 一个额外的作用：代码保护
* 建议每个文件是一个module，所以建议用install来配置docker
* Cython 互相引用会出很多问题
* 很多时候用intel编译器，有时候会出问题
* [例子](https://github.com/rwbfd/ml-training-camp/blob/main/chap02/cython_example.ipynb), 先把.pyx代码编译成cpp文件然后生成.so文件
* 优先写C++
* 可以绕过GIL的限制，加速python代码但是不能优化内存
* 资源分配和释放在一个地方，要么在Python要么在C，不要C创建资源然后用Python释放
#### 并行
* 先用Profiler再找算法本身的问题
* 不要上来就并行，并行有很多代价
* 并行建议用SIMD不要多线程
* 需要并行的时候用Ray，[例子](https://github.com/rwbfd/ml-training-camp/tree/main/chap02/ray)
* OpenMP 可以写C代码但是不能写python的任何代码, 不推荐使用。[例子](https://github.com/rwbfd/ml-training-camp/blob/main/chap02/openmp/openmp_demo.pyx)
