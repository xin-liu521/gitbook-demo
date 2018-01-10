### 新增客户任务

###### 接口说明:
用户客户任务新增表单数据提交。

###### 请求方式： POST

###### 请求地址： 

http://ip:port/SmartCRM/api/mydayreport/addtask

###### 请求报文：
```
{
    "customid":"123",
    "customerName":"123",
    "projectCode":"H11Chh88888",
    "projectName":"项目名称",
    "taskowner":"renliangd",
    "tasktype":"任务类型",
    "taskfreq":"跟踪频率",
}
```

###### 参数说明：

参数 | 必须 | 说明
---|---|---
customid | 是 | 客户ID
customerName | 是 | 客户名称
projectCode | 是 | 项目编号
projectName | 是 | 项目名称
taskowner | 是 | 用户ITCode
tasktype | 是 | 日报类型编码 客户拜访：1，客户收款：4，其他：6
taskfreq | 是 | 跟踪频率 1-9 日，周，月，季，明年，不跟踪，本周不，本月不，本季不
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
