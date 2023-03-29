# Product Available Date And Price

### Description

According to the `product id`, get the list of product sales dates,

### API URL

    /v2/product/availabilities

### Parameter

| parameter           | type          | required | Description             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  yes   | product id  |

### Reqeust parameter example

    {
    	"product_id":101686926
    }

### Response

    Tour package：
    {
        "code": 0,
        "msg": "success",
        "data": {
            "currency": "USD",
            "symbol": "$",
            "price": {
                //single room price
                "single": "1295.0000",
                //double room price
                "double": "881.0000",
                //triple room price
                "triple": "797.0000",
                //quad room price
                "quad": "755.0000",
                //kid price
                "kid": "631.0000"
            },
            "availabilities": [
                {
                    "date": "2018-01-17",
                    "display_price": 325,
                    "min_persons": 1
                },
                {
                    "date": "2018-01-22",
                    "display_price": 325,
                    "min_persons": 1
                }
            ]
        }
    }


