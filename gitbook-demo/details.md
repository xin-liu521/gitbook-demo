### 日报详情查询

###### 接口说明:
根据客户ID及日期查询某客户的第一条待处理任务或者根据任务ID查询某个任务的详细信息。

###### 请求方式： GET

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/details?customid=1&taskId=12&date=2018-01-08

###### 参数说明：

参数 | 必须 | 说明
---|---|---
customid | 否 | 客户ID
date | 否 | 日期
taskId | 否 | 任务ID

###### 返回报文：

```
{
    "data": {
        "taskId":"任务ID",
        "taskName":"任务名称",
        "tasktype":"任务类型ID",
        "projectName":"项目名称"
        .......
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
taskName | 是 | 任务名称
tasktype | 是 | 任务类型ID
projectName | 是 | 项目名称

