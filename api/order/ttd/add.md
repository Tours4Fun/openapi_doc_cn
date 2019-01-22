# Create Order

### Description

    Create Order

### API address

    api_open/order/add

### Request parameter description

| Parameter           | Type          | Is required  | Description             |
| ------------------- |:-------------:| ------------:| :-----------------------|
| product_id          | int           |     Yes      |   Product id         |
| departure_date      | date          |     Yes      |   Travel date          |
| departure_address   | string        |     Yes      |   Departure address [Choose from departure](../../product/ttd/detail.md#product_departure)|
| end_address         | string        |     Yes      |   End address|
| sku_info            | array         |     Yes      |   --|
| -sku_id             | int           |     Yes      |   Sku id|
| -count              | int           |     Yes      |   The number of sku purchases|
| contact             | array         |     Yes      |   Subscriber contact information|
| -first_name         | string        |     Yes      |   Subscriber first name|
| -last_name          | string        |     Yes      |   Subscriber end name|
| -email              | string        |     Yes      |   Subscriber email|
| -mobile             | string        |     Yes      |   Subscriber mobile|
| guest_info          | --            |     If passenger is not empty => Yes      |   Traveler information|
| -sku_id             | int           |     Yes      |   Sku id|
| -firstname_en       | string        |              |   Traveler first name |
| -lastname_en        | string        |              |   Traveler lase name|
| -gender             | -             |    [男=>1, 女=>2]       |   Traveler gender|
| -dob                | -             |              |   Traveler date of birth|
| -weight             | -             |              |   Traveler weight|
| -passport           | -             |              |   Traveler passport|
| -mobile             | -             |              |   Traveler mobile|

### Request parameter demo

	{
        "product_id":102851724,          
        "departure_date":"2019-01-22",
        "departure_address":"jhjhj",
        "end_address":"jhjhj",
        "sku_info":[
            {
                "sku_id":760,
                "count":1
            },
            {
                "sku_id":761,
                "count":1
            }
        ],
        "contact":{
            "first_name": "Sagar",
            "last_name": "Thesia",
            "email": "sagart.bipl@gmail.com",
            "mobile": "9574775177"
        },
        "guest_info":[
            {
                "type": "SAGAR Great Value",
                "sku_id": 760,
                "lastname_en": "Thesia",
                "firstname_en": "Sagar",
                "gender": 1,
                "dob": "1979-12-26",
                "weight": 100,
                "passport": "98765432",
                "mobile": "1-9574775177"
            },
            {
                "type": null,
                "sku_id": 761,
                "lastname_en": "Chandresh",
                "firstname_en": "BIPL",
                "gender": 1,
                "dob": "1991-12-05",
                "weight": 5,
                "passport": "sdfeed",
                "mobile": "1-4561237890"
            }
        ]
    }	

### Return field description

| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| order_id                          |     Order id                            |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "order_id": 10004052
        }
    }


