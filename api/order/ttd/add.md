# Create Order

### Description

    Create Order

### API address

    ttd/order/add

### Request parameter description

| Parameter           | Type          | Is required  | Description             |
| ------------------- |:-------------:| ------------:| :-----------------------|
| product_id          | int           |     Yes      |   Product id         |
| departure_date      | date          |     Yes      |   Travel date          |
| departure_address   | string        |     Yes      |   Departure address [Choose from departure of product detail info]|
| end_address         | string        |     Yes      |   End address [Choose from departure of product detail info]|
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
| -ext_fields         | array         |     Yes, If bookingInfo.passenger_level is not empty |   Traveler additional booking Fields for Guest SKU.|
| ext_fields          | array         |     Yes, If bookingInfo.product_level is not empty |   Product additional booking Fields for all selected SKUs |

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
                "mobile": "1-9574775177",
                "ext_fields": {
                    "您的早餐要求": "水果或一些健康食品.",
                    "您想重复哪项服务？": "水疗和健身房"
                }
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
                "mobile": "1-4561237890",
                "ext_fields": {
                    "高度 (cm)": "180",
                    "您的早餐要求": "我会吃午饭"
                }
            }
        ],
        "ext_fields": {
            "你想带Spa吗？": "Yes",
            "酒店的特殊要求": "不，没有"
        }
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


