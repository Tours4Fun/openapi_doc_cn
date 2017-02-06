# 文档信息

**最后更新日志：** 2017-01-23

**VERSION：**`BETA`

**查看修改记录：** [这里查看](updatelog.md)

# APPKEY 申请
在调用相关API前，请先向我们商务申请途风开放平台APPKEY，并开通对应权限后方能调用API。

**Secret Key:**

    SECRET_KEY秘钥随APPKEY一并发放，请妥善保管该秘钥，不要泄露。该秘钥为服务端签名验证重要凭据，
    具体API调用方式请看下一章。

# API 调用

## 网关地址:

    https://openapi.tufengwang.com

## API调用

### 请求协议

API调用使用HTTP协议，`POST`方法进行调用，网关只支持`POST`调用，请注意。

### 请求参数

API调用时，参数使用`JSON`方式表示，并作为Http Body 附加在http请求中。
同时HTTP HEADER中加入`Content-Type: application/json; charset=utf-8`。

例如：

```javascript
{
    "product_id":123
}
```

### 系统参数

系统参数使用 `GET` 方式将参数以form-urlencoed的方式附加在api url后面，例如：

    https://openapi.tufengwang.com/v1/product/detail?appkey=xxxxxx&sign=xxxxx&t=xxxxx&lang=zh_tw


**系统参数列表:**

| 参数名    | 数据类型 |             说明               |
| :------: |:--------:|:------------------------------:|
| appkey   |  string  | 应用标识，开通访问权限时分配   |
| t        |  int     | timestamp时间戳，与服务器时间相差必须10分钟内。   |
| sign     |  string  | 参数签名值，由appkey,t, 请求参数一并得到。|
| lang     |  string  | 可选,语言选项,取值 zh\_cn 、 zh\_tw 。|


### 签名算法

签名算法主要用于生成系统参数 `sign`。生成方式为：

    md5(appkey + t + appsecret + 请求参数(json字符串))
[签名范例](./api/sign_usage.md)

## 标准调用返回

HTTP CODE 不管是否错误，均返回 200，由具体返回内容确定正确或错误。

```javascript
{
    "code" : 0, //状态码，0 表示成功， 非0表示错误码
    "msg" : "", //消息信息，成功默认 "success"，其它代表错误信息
    "data" : {}, //数据内容，由API确定，可能是数组、字符串、数组、对象等。
}
```

# 重点数据结构

| 数据     | 中文名  |             说明               |
| :------: |:--------:|:------------------------------:|
| [产品(product)](./datastruct/product.md)  |  产品  | 产品数据结构，产品根据产品线不同，会有不同的数据结构。   |



# API列表

----


| API类别    |  地址   |
| ---------- |:--------:|
|  产品API   | [前往查看](./api/product.md) |
|  订单API   | [前往查看](./api/order.md) |
