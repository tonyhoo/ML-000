> 在 天眼查/企查查 等企业查询平台中，搜索企业相关的结构化数据，提取变量特征（至少100个）

| API            | Feature                           | Description                       |
|----------------|-----------------------------------|-----------------------------------|
| BaseInfo       | historyNames                      | 曾⽤名                            |
| BaseInfo       | regStatus                         | 企业状态                          |
| BaseInfo       | cancelDate                        | 注销⽇期                          |
| BaseInfo       | regCapital                        | 注册资本                          |
| BaseInfo       | staffNumRange                     | ⼈员规模                          |
| BaseInfo       | industry                          | ⾏业                              |
| BaseInfo       | bondNum                           | 股票号                            |
| BaseInfo       | type                              | 法⼈类型，1 ⼈ 2 公司             |
| BaseInfo       | bondName                          | 股票名                            |
| BaseInfo       | revokeDate                        | 吊销⽇期                          |
| BaseInfo       | legalPersonName                   | 法⼈                              |
| BaseInfo       | revokeReason                      | 吊销原因                          |
| BaseInfo       | regNumber                         | 注册号                            |
| BaseInfo       | property3                         | 英文名                            |
| BaseInfo       | creditCode                        | 统一社会信用代码                  |
| BaseInfo       | usedBondName                      | 股票曾用名                        |
| BaseInfo       | fromTime                          | 经营开始时间                      |
| BaseInfo       | approvedTime                      | 核准时间                          |
| BaseInfo       | socialStaffNum                    | 参保人数                          |
| BaseInfo       | alias                             | 简称                              |
| BaseInfo       | companyOrgType                    | 企业类型                          |
| BaseInfo       | id                                | 企业id                            |
| BaseInfo       | orgNumber                         | 组织机构代码                      |
| BaseInfo       | cancelReason                      | 注销原因                          |
| BaseInfo       | toTime                            | 经营结束时间                      |
| BaseInfo       | actualCapital                     | 实收注册资金                      |
| BaseInfo       | estiblishTime                     | 成立日期                          |
| BaseInfo       | regInstitute                      | 登记机关                          |
| BaseInfo       | taxNumber                         | 纳税人识别号                      |
| BaseInfo       | businessScope                     | 经营范围                          |
| BaseInfo       | regLocation                       | 注册地址                          |
| BaseInfo       | tags                              | 企业标签                          |
| BaseInfo       | name                              | 企业名                            |
| BaseInfo       | bondType                          | 股票类型                          |
| BaseInfo       | percentileScore                   | 企业评分                          |
| BaseInfo       | industryAll_categoryMiddle String | 国⺠经济行业分类中类              |
| BaseInfo       | industryAll_categoryBig           | 国⺠经济行业分类大类              |
| BaseInfo       | industryAll_category              | 国⺠经济行业分类⻔类              |
| BaseInfo       | isMicroEnt                        | 是否是小微企业 0不是 1是          |
| BaseInfo       | base                              | 省份简称                          |
| CommercialInfo | investList_regStatus              | 企业状态                          |
| CommercialInfo | investList_amount                 | 投资金额(万)                      |
| CommercialInfo | investList_estiblishTime          | 开业时间                          |
| CommercialInfo | investList_regCapital             | 注册资金                          |
| CommercialInfo | investList_type                   | 1-公司 2-人                       |
| CommercialInfo | investList_percent                | 投资占比                          |
| CommercialInfo | investList_legalPersonName        | 法人                              |
| CommercialInfo | investList_business_scope         | 经营范围                          |
| CommercialInfo | investList_orgType                | 公司类型                          |
| CommercialInfo | investList_creditCode             | 统一社会信用代码                  |
| CommercialInfo | investList_name                   | 被投资公司                        |
| CommercialInfo | investList_alias                  | 简称                              |
| CommercialInfo | investList_id                     | 公司id                            |
| CommercialInfo | investList_category               | 行业                              |
| CommercialInfo | investList_personType             | 1 人 2 公司                       |
| CommercialInfo | investList_base                   | 省份简称                          |
| CommercialInfo | staffList_staffTypeName           | 主要人员职位                      |
| CommercialInfo | staffList_name                    | 主要人员名称                      |
| CommercialInfo | staffList_logo                    | logo                              |
| CommercialInfo | staffList_id                      | graphId                           |
| CommercialInfo | staffList_type                    | 主要人员类型 1-公司 2-人          |
| CommercialInfo | staffList_typeJoin                | 职位                              |
| CommercialInfo | liquidatingInfo_manager           | 清算信息_清算组负责人             |
| CommercialInfo | liquidatingInfo_member            | 清算信息_清算成员名称             |
| CommercialInfo | liquidatingInfo_id                | 清算信息_表id                     |
| CommercialInfo | illegalList_removeDate            | 严重违法_移出时间                 |
| CommercialInfo | illegalList_fact                  | 严重违法_违法事实                 |
| CommercialInfo | illegalList_putReason             | 严重违法_列入原因                 |
| CommercialInfo | illegalList_putDepartment         | 严重违法_决定列入机关             |
| CommercialInfo | illegalList_removeDepartment      | 严重违法_决定移出机关             |
| CommercialInfo | illegalList_removeReason          | 严重违法_移出原因                 |
| CommercialInfo | illegalList_id                    | 严重违法_表id                     |
| CommercialInfo | illegalList_type                  | 严重违法_类别                     |
| CommercialInfo | illegalList_putDate               | 严重违法_列入时间                 |
| CommercialInfo | abnormalList_removeDate           | 经营异常列表_移出时间             |
| CommercialInfo | abnormalList_putReason            | 经营异常列表_列入原因             |
| CommercialInfo | abnormalList_putDepartment        | 经营异常列表_决定列入机关         |
| CommercialInfo | abnormalList_removeDepartment     | 经营异常列表_移出机关             |
| CommercialInfo | abnormalList_removeReason         | 经营异常列表_移出原因             |
| CommercialInfo | abnormalList_id                   | 经营异常列表_表 id                |
| CommercialInfo | abnormalList_putDate              | 经营异常列表_列入时间             |
| CommercialInfo | punishList_departmentName         | 行政处罚_作出行政处罚决定机关名称 |
| CommercialInfo | punishList_regNumber              | 行政处罚_注册号                   |
| CommercialInfo | punishList_punishNumber           | 行政处罚_行政处罚决定书文号       |
| CommercialInfo | punishList_name                   | 行政处罚_公司名称                 |
| CommercialInfo | punishList_publishDate            | 行政处罚_公示日期                 |
| CommercialInfo | punishList_description            | 行政处罚_描述                     |
| CommercialInfo | punishList_id                     | 行政处罚_表 id                    |
| CommercialInfo | punishList_type                   | 行政处罚_违法行为类型             |
| CommercialInfo | punishList_content                | 行政处罚_行政处罚内容             |
| CommercialInfo | punishList_base                   | 行政处罚_省份简称                 |
| CommercialInfo | punishList_legalPersonName        | 行政处罚_法定代表人(负责人)姓名   |
| CommercialInfo | punishList_decisionDate           | 行政处罚_作出行政处罚决定日期     |
| CommercialInfo | mortList_amount                   | 动产抵押_被担保债权数额           |
| CommercialInfo | mortList_cancelDate               | 动产抵押_注销日期                 |
| CommercialInfo | mortList_detail                   | 数量、质量、状况、所在地等情况    |
| CommercialInfo | mortList_pawnName                 | 动产抵押_名称                     |
| CommercialInfo | mortList_ownership                | 动产抵押_所有权归属               |
| CommercialInfo | mortList_remark                   | 动产抵押_备注                     |

