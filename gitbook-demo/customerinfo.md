### 项目列表数据查询

###### 接口说明:
根据关键字查询客户列表信息。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/customerinfo?keywords=&maxSize=10

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
            {"customid"："1","customName":"中信银行"},
            {"customid"："2","customName":"国开行"}
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
customid | 是 | 客户ID
customName | 是 | 客户名称
