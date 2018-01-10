### 项目列表数据查询

###### 接口说明:
根据关键字查询项目基本信息。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/projectinfo?keywords=&maxSize=10

###### 参数说明：

参数 | 必须 | 说明
---|---|---
keywords | 是 | 检索关键字
maxSize | 否 | 最大结果集

###### 返回报文：

```
{
    "data": {
        "total":"100",
        "rows":[
            {"projectCode"："1","projectName":"CRM"},
            {"projectCode"："2","projectName":"NPMC"}
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
projectCode | 是 | 项目编号
projectName | 是 | 项目名称
