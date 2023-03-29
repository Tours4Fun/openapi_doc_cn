# Product Departure Location

### Description

Obtain the departure location of the product according to the `product id` and `departure date`


### API URL

    /v2/product/departure

### Parameter

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  yes   | product id  |
| departure_date     | date  |  yes   | departure date(Y-m-d)  |

### Request parameter example

    {
    	"product_id" : 101457621,
    	"departure_date" : "2018-01-12"
    }

### Response

	{
        "code": 0,
        "msg": "success",
        "data": [
            {
                //departure_id
                "id": 32903,
                "start_time": "11:00:00",
                "end_time": "",
                "location": "12121",
                "address": "12212112",
                "tips": "12211222"
            },
            {
                "id": 32902,
                "start_time": "12:00:00",
                "end_time": "",
                "location": "Location",
                "address": "Full Address",
                "tips": "Tips\tTips"
            }
        ]
    }

