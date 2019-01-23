# Cancel order

### Description

    cancle order

### API address

    api_open/order/cancel

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| order_id                | int           |     Yes      |   Order id         |
| cancel_reason                | string           |     Yes      |   Cancel order reason         |


### Request parameter demo

	{
    	"cancel_reason":"不想要了",
    	"order_id":10004051
    }

### Return field description

### Interface return

	{
        "code": 0,
        "msg": "cancel order success",
        "data": {
            "cancel_reason": "不想要了",
            "order_id": 10004051
        }
    }


