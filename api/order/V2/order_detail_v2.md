# Order detail

**Description**

Get order detail by order_id

### API URL

    POST   /v2/order/detail

**Parameter**

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| -----------------:|
| order_id    | integer  |  yes   | order id   |

**Response**

| parameter           | type          | description             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 success, fail|
| msg  | string | success |
| data | array |  array or empty array |
| -order_id | integer | order id |
| -order_status | integer |  order status |
| -created_at | datetime |  order purchase time |
| -updated_at | datetime |  order update time |
| -price      | double   |  order price |
| -product_list | array |  product list |
| ---product_id | integer |  product id |
| ---product_name | string | product name |
| ---product_status | integer |  order product status |
| ---product_line   | string |  product line |
| ---departure_date  | date |  order departure date |
| ---end_date        | date | order end date   |
| ---departure_address | string | departure address |
| ---rooms              | array   |  room info |
| ----adult            | integer |  adult number |
| ----kid              | integer |  kid number |
| ----single_pairup    | integer |  single pairup |
| ---price_info    | array |  price info |
| ----total_retail         | double |  total price |
| ----total_retail_target_currency | double |  target currency total price |
| ----original_total_retail        | double |  origin total price |
| ----original_total_retail_target_currency | double |  target currency origin price |
| ----total_discount       | double |  total discount price |
| ----total_discount_target_currency        | double |  target currency total discount price |
| ---contact          | array     |  contact info|
| ----first_name      | string   |  first name|
| ----last_name       | string   |  last name|
| ----mobile          | string   |  mobile|
| ----email           | string   |  email|
| ---guest            | string   |  guest info|
| ---upgrades         | string   |  upgrades info |
| ----upgrade_id      | integer   |  upgrade id|
| ----option_id       | integer   |  upgrade option id|
| ----name            | string   |  upgrade name|
| ----subname         | string   |  upgrade sub name|
| ----option_name         | string   |  upgrade option name|
| ----provider_tour_code  | string   |  provider tour code|

**Reqeust parameter example**
```
{
    "order_id":1672
}
```

**Response**
```
{
    "code": 0,
    "msg": "success",
    "data": {
        "order_id": 10003997,
        "order_status": 100,
        "created_at": "2019-01-16 19:42:48",
        "updated_at": "2019-01-16 19:42:50",
        "price": 2040.06,
        "product_list": [
            {
                "product_id": 101457594,
                "product_name": "[weff's annual hits] (4 days) in-depth tour of Los Angeles and themed projects: choose three of the eight themed projects",
                "product_status": 10000,
                "product_line": "tour",
                "departure_date": "2019-01-20",
                "end_date": "2019-01-20",
                "departure_address": "jhjhj",
                "rooms": [
                    {
                        "adult": 2,
                        "kid": 0,
                        "single_pairup": 1
                    }
                ],
                "price_info": {
                    "total_retail": 1285.2,
                    "total_retail_target_currency": 1496.5068,
                    "original_total_retail": 1752,
                    "original_total_retail_target_currency": 2040.0559,
                    "total_discount": 466.8,
                    "total_discount_target_currency": 543.5491
                },
                "contact": [
                    {
                        "firstname": "a",
                        "lastname": "b",
                        "telephone": "1",
                        "email": "2@q.q"
                    }
                ],
                "guest": [
                    {
                        "order_product_guest_id": 6293,
                        "order_product_id": 46318,
                        "telephone": null,
                        "email": null,
                        "type": "adult",
                        "firstname_en": "ghghg",
                        "mobile": "86-6767"
                    },
                    {
                        "order_product_guest_id": 6294,
                        "order_product_id": 46318,
                        "telephone": null,
                        "email": null,
                        "type": "kid",
                        "firstname_en": "oooo",
                        "mobile": "86-67887"
                    }
                ],
                "upgrades": [
                    {
                        "upgrade_id": 3,
                        "option_id": 3,
                        "name": "airport pick up",
                        "subname": "",
                        "option_name": "Quotation is required for more people",
                        "provider_tour_code": ""
                    },
                    {
                        "upgrade_id": 9,
                        "option_id": 60,
                        "name": "hotel upgrades",
                        "subname": "",
                        "option_name": "Westin Bonaventure Downtown Los Angeles",
                        "provider_tour_code": ""
                    }
                ]
            }
        ]
    }
}
```
