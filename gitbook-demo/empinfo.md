### 项目列表数据查询

###### 接口说明:
根据关键字模糊检索公司人员摘要信息。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/empinfo?keywords=&maxSize=10

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
            {"itcode"："zhangdig","empName":"张迪","deptName":"业务解决方案部"},
            {"itcode"："renliangd","empName":"任亮","deptName":"PMO"}
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
itcode | 是 | 员工ITCODE
empName | 是 | 姓名
deptName | 是 | 部门
