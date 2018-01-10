### 日报表单提交

###### 接口说明:
保存用户提交的日报表单数据接口，接口根据任务类型判断是那种类型的任务，不同的任务类型请求的表单数据类型不同。

###### 请求方式： POST

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/save

###### 请求报文：
```
{
    "taskId":"123",
    "tasktype":"1",
    "taskName":"任务名称",
    "itcode":"renliangd",
    "projectCode":"项目编号",
    "projectName":"项目编号",
    ......
}
```

###### 参数说明：

参数 | 必须 | 说明
---|---|---
taskId | 是 | 任务ID
taskName | 是 | 任务名称
tasktype | 是 | 日报类型编码
itcode | 是 | 员工ITCODE
projectCode | 是 | 项目编号
projectName | 是 | 项目名称
... | ... | ...

###### 返回报文：

```
{
    "rtnCode": "2000",
    "rtnMsg": "保存成功！",
    "data": {}
}
```

###### 返回说明：

参数 | 必须 | 说明
---|---|---
rtnCode | 是 | 返回码
rtnMsg | 是 | 返回消息
data | 是 | 返回数据
