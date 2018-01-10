### 项目列表数据查询

###### 接口说明:
根据关键字及行方名称模糊检索银行人员摘要信息。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/empinfo?keywords=&maxSize=10&bankname=

###### 参数说明：

参数 | 必须 | 说明
---|---|---
keywords | 否 | 检索关键字
maxSize | 否 | 最大结果集
bankname | 是 | 银行名称

###### 返回报文：

```
{
    "data": {
        "total":"100",
        "rows":[
            {"customerid":"68",custname"："李海宁","custmerdept":"软件开发部","custpost":"副处长"},
            {"customerid":"68","custname"："李海宁","custmerdept":"软件开发部","custpost":"副处长"}
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
customerid | 是 | 客户干系人ID
custname | 是 | 客户干系人姓名
custmerdept | 是 | 部门
custpost | 是 | 职务
