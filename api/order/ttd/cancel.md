# Cancel order

### Description

    cancle order

### API address

    ttd/order/cancel

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

    success
    
	{
        "code": 0,
        "msg": "cancel order success",
        "data": {
            "cancel_reason": "不想要了",
            "order_id": 10004051
        }
    }
    
    error 1.
        {
            "code": 30007,
            "msg": "Cancel Order failed!",
            "data": []
        }
    Solution:Please check the order status or contact us.
    
    error 2.   
        {
            "code": 30007,
            "msg": "Permission Not Allow",
            "data": []
        }
    Solution:The order does not belong to you, please check the order id.


