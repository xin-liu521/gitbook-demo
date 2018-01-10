### 日报查询

###### 接口说明:
用于根据日期、任务类型、关键字查询日报包括已处理和未处理的日报信息，仅查询日报类型为客户拜访，收款、其他三个类型的任务，支持分页查询。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/query?currentPage=1&showCount=10&date=2018-01-08&itcode=renliangd&tasktype=1

###### 参数说明：

参数 | 必须 | 说明
---|---|---
currentPage | 是 | 当前页
showCount | 是 | 每页行数
date | 是 | 查询日期
itcode | 是 | 用户ITCode
tasktype | 是 | 日报类型编码

###### 返回报文：

```
{
    "data": {
        "total":"100",
        "rows":[
            {"taskId"："1","displayText":"左小强2017171230/zuoxq/中区事业部"},
            {"taskId"："1","displayText":"左小强2017171231/zuoxq/中区事业部"},
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
total | 是 | 总行数，整型
rows | 是 | 数据列表
taskId | 是 | 任务ID
displayText | 是 | 列表显示文本
