# Order detail

### Description

    Get the order detail

### API address

    api_open/order/detail

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
| order_status                      |     [Click to view](../../../README.md)[订单状态码]                             |
| created_at                        |     Order create time                                  |
| updated_at                        |     Order modify time                            |
| price                             |     Order amount[USD]           |
| product_list                      |     Order related products                            |
| -product_id                       |     Product id               |
| -product_name                     |     Product name                                |
| -product_status                   |     [Click to view](../../../README.md)[订单产品状态码]                                |
| -departure_date                   |     Travel time                           |
| -end_date                         |     Travel end time                                |
| -departure_address                |     Departure address                          |
| -price_info                       |     --                                            |
| --total_retail                    |     Total amount of this product                                  |
| --currency                        |     Product currency                                  |
| --symbol                          |     Currency symbol                                   |
| -contact                          |     --                                            |
| --firstname                       |     First name                                  |
| --lastname                        |     Last name                                  |
| --telephone                       |     Telephone                                  |
| -guest                            |     Traveler information                                            |
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
| --amount                          |     Purchase quantity                      |
| --price                           |     The total price of this sku                      |
| --display_name                    |     Display name                      |
| --sku_name                        |     Sku name                      |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "order_id": 10004051,
            "order_status": 100,
            "created_at": "2019-01-21 14:34:36",
            "updated_at": "2019-01-21 14:34:38",
            "price": 15.77,
            "product_list": [
                {
                    "product_id": 102851724,
                    "product_name": "123123",
                    "departure_date": "2019-01-22",
                    "end_date": "2019-01-22",
                    "departure_address": "jhjhj",
                    "price_info": {
                        "total_retail": 22,
                        "currency": "AUD",
                        "symbol": "AUD"
                    },
                    "contact": [
                        {
                            "firstname": "Sagar",
                            "lastname": "Thesia",
                            "telephone": "9574775177",
                            "email": "sagart.bipl@gmail.com"
                        }
                    ],
                    "guest": [
                        {
                            "telephone": "",
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
                            "telephone": "",
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
                            "sku_id": 760,
                            "amount": 1,
                            "price": 11,
                            "display_name": "666",
                            "sku_name": "成人"
                        },
                        {
                            "sku_id": 761,
                            "amount": 1,
                            "price": 11,
                            "display_name": "999",
                            "sku_name": "儿童"
                        }
                    ]
                }
            ]
        }
    }


