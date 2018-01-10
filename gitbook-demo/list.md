### 日报首页查询

###### 接口说明:
用于日报首页数据加载获取客户经理待处理的日报列表根据客户分组，仅查询日报类型为客户拜访，收款、其他三个类型的任务，支持分页查询。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/list?currentPage=1&showCount=10&date=2018-01-08&itcode=renliangd

###### 参数说明：

参数 | 必须 | 说明
---|---|---
currentPage | 是 | 当前页
showCount | 是 | 每页行数
date | 是 | 查询日期
itcode | 是 | 用户ITCode

###### 返回报文：

```
{
    "data": {
        "headMsg":"当前状态存在8个待处理任务，1个领导指示",
        "yeaterdayIsFinish":"Y",
        "total":"100",
        "rows":[
            {"customid"："1","customerName":"中信银行",taskCount":"10","logo":"ddddddd"},
            {"customid"："2","customerName":"民生银行","taskCount":"10","logo":"ddddddd"}
        ]
    },
    "rtnMsg": "查询成功！",
    "rtnCode": "2000"
}
```

###### 返回说明：

参数 | 必须 | 说明
---|---|---
rtnCode | 是 | 返回码
rtnMsg | 是 | 返回消息
data | 是 | 返回数据
headMsg| 是 | 顶部提示消息
yeaterdayIsFinish| 是 | 当前日期的前一天是否有未处理的任务，是：Y，否：N
total | 是 | 总行数，整型
rows | 是 | 数据列表
customid | 是 | 客户ID
customerName | 是 | 客户名称
taskCount | 是 | 当前客户任务数,整型
logo | 是 | 客户企业LOGO图片BASE64码

