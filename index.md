# APPKEY 申请
在调用相关API前，请先向我们商务申请途风开放平台APPKEY，并开通对应权限后方能调用API。

**Secret Key:**

    SECRET_KEY秘钥随APPKEY一并发放，请妥善保管该秘钥，不要泄露。该秘钥为服务端签名验证重要凭据，
    具体API调用方式请看下一章。

# API 调用

## 网关地址:

    https://openapi.toursforfun.com/v1

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

    https://openapi.toursforfun.com/v1/product/detail?appkey=xxxxxx&sign=xxxxx&t=xxxxx

**系统参数列表:**

| 参数名    | 数据类型 |             说明               |
| :------: |:--------:|:------------------------------:|
| appkey   |  string  | 应用标识，开通访问权限时分配   |
| t        |  int     | timestamp时间戳，与服务器时间相差必须10分钟内。   |
| sign     |  string  | 参数签名值，由appkey,t, 请求参数一并得到。|


### 签名算法

签名算法主要用于生成系统参数 `sign`。生成方式为：

    md5(appkey + t + secretkey + 请求参数(json字符串))

# 重点数据结构

| 数据     | 中文名  |             说明               |
| :------: |:--------:|:------------------------------:|
| [product](./datastruct/product.md)  |  产品  | 产品数据结构，产品根据产品线不同，会有不同的数据结构。   |

## 产品


# API列表

----

## 产品API

| API                                         |  请求方法 |说明          |
| ------------------------------------------- |:--------:|:-------------:|
| [创建订单](./doc/api_order/order_create.md)  |   POST   |   创建订单    |