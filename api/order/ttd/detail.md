# Order detail

### Description

    Get the order detail

### API address

    ttd/order/detail

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| order_id                | int           |     Yes      |   Order id         |


### Request parameter demo

	{
    	"order_id":10004051
    }

### Return field description

| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| order_id                          |     Order id                             |
| order_status                      |     Order status[100,200,300]                             |
| order_status_name                 |     Order status name[预定中,已出票,已取消]                            |
| created_at                        |     Order create time                                  |
| updated_at                        |     Order modify time                            |
| price                             |     Order amount[USD]           |
| product_list                      |     Order related products                            |
| -product_id                       |     Product id               |
| -product_name                     |     Product name                                |
| -departure_date                   |     Travel time                           |
| -end_date                         |     Travel end time                                |
| -departure_address                |     Departure address                          |
| -end_address                      |     End address                          |
| -contact                          |     --                                            |
| --firstname                       |     First name                                  |
| --lastname                        |     Last name                                  |
| --telephone                       |     Telephone                                  |
| -guest_info                       |     Traveler information                                            |
| --email                           |     Email                                            |
| --sku_id                          |     Sku id                                            |
| --lastname_en                     |     Last name                                            |
| --firstname_en                    |     First name                                            |
| --gender                          |     Gender[1=>Male, 2=>Female]                                            |
| --dob                             |     Date of birth                                            |
| --weight                          |     Weight                                            |
| --passport                        |     Passport                                            |
| --mobile                          |     Mobile                                            |
| -detail                           |     Product sku detail                                  |
| --sku_id                          |     Sku id                                  |
| --count                           |     Purchase quantity                      |
| --display_name                    |     Display name                      |
| --sku_name                        |     Sku name                      |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "order_id": 10004060,
            "order_status": 100,
            "order_status_name": "预定中",
            "created_at": "2019-01-23 17:15:51",
            "updated_at": "2019-01-23 17:15:51",
            "price": 54.73,
            "currency": "USD",
            "product_list": [
                {
                    "product_id": 102851680,
                    "product_name": "Testing Alpesh product",
                    "departure_date": "2019-01-25",
                    "end_date": "2019-01-25",
                    "departure_address": "jhjhj",
                    "end_address": "hhhh",
                    "contact": [
                        {
                            "firstname": "Sagar",
                            "lastname": "Thesia",
                            "telephone": "9574775177",
                            "email": "sagart.bipl@gmail.com"
                        }
                    ],
                    "guest_info": [
                        {
                            "email": "",
                            "sku_id": "760",
                            "lastname_en": "Thesia",
                            "firstname_en": "Sagar",
                            "gender": "1",
                            "dob": "1979-12-26",
                            "weight": "100",
                            "passport": "98765432",
                            "mobile": "1-9574775177"
                        },
                        {
                            "email": "",
                            "sku_id": "761",
                            "lastname_en": "Chandresh",
                            "firstname_en": "BIPL",
                            "gender": "1",
                            "dob": "1991-12-05",
                            "weight": "5",
                            "passport": "sdfeed",
                            "mobile": "1-4561237890"
                        }
                    ],
                    "detail": [
                        {
                            "sku_id": 553,
                            "count": 1,
                            "display_name": "2b",
                            "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                        },
                        {
                            "sku_id": 554,
                            "count": 1,
                            "display_name": "",
                            "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                        }
                    ]
                }
            ]
        }
    }


