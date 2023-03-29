# Cancel order

**Description**

Cancel order

### API URL

    POST   /v2/order/cancel

**Parameter**

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| -----------------:|
| order_id    | integer  |  yes   | order id   |
| cancel_reason | string  |  no   | reason for cancellation   |

**Response**

| parameter           | type          | description             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 success, fail|
| msg  | string | success |
| data | array |  array or empty array |
| -order_id | integer |  order id |
| -cancel_reason | string |  reason for cacellation |

**Reqeust parameter example**
```
{
    "order_id":1672
    "cancel_reason":"I don't want to buy it now"
}
```

**Response**
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
       "cancel_reason":"I don't want to buy it now"
	}
}
```
