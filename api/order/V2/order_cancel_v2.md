# 订单详情

**描述**

根据订单号，获取订单详情信息

### API地址

    POST   /v2/order/cancel
	
**参数**

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| -----------------:|
| order_id    | integer  |  是   | 订单ID   |
| cancel_reason | string  |  否   | 取消原因   |

**返回**

| 参数           | 类型          | 描述             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 成功, 失败| 
| msg  | string | success |
| data | array |  数组 或 空数组 |
| -order_id | integer |  订单ID |
| -cancel_reason | string |  取消原因 |
	
**请求参数示例**
```
{
    "order_id":1672
    "cancel_reason":"不想买了"
}
```

**返回示例**
```
{
	"code": 30007,
	"msg": "This order can not cancelled after paid",
	"data": {}
}
or
{
	"code": 0,
	"msg": "cancel order success",
	"data": {
	   "order_id":1672
       "cancel_reason":"不想买了"
	}
}
```
