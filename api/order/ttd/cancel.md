# Cancel order

### Description

    cancle order

### API address

    api_open/order/cancel

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| orderId                | int           |     Yes      |   Order id         |
| cancelReason                | string           |     Yes      |   Cancel order reason         |


### Request parameter demo

	{
    	"cancelReason":"不想要了",
    	"orderId":10004051
    }

### Return field description

### Interface return

	{
        "code": 0,
        "msg": "cancel order success",
        "data": {
            "cancelReason": "不想要了",
            "orderId": 10004051
        }
    }


