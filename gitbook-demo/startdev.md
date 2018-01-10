### 术语与简写
- SmartCRM： 销售客户管理系统
- 移动端： 企业微信
- NPMC系统：NPMC项目辅助管理系统

### 接口说明

SmartCRM系统与企业微信接口接入采用HTTP协议,交互报文为JSON。

### GET方式调用

GET方式调用时采用查询字符串传参即URL传参的方式
- 请求方式：get
- 请求URL：http://ip:port/SmartCRM/api/mydayreport/query?id=123

### POST方式调用

POST请求调用时采用请求体传参，NPMC系统规定以下结构请求json报文
- 请求方式：post
- 请求URL：http://ip:port/SmartCRM/api/mydayreport/save
- 请求报文

```
{

}
```

- 返回报文

```
{
    "rtnCode":"2000",
    "rtnMsg":"成功",
    "data": {
        
    }
}
```

- 返回说明

参数 | 必须 | 说明
---|---|---
rtnCode | 是 | 返回码
rtnMsg | 是 | 消息
data | 是 | 响应业务报文