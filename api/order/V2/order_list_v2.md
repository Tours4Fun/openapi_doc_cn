# Order list

**Description**

Get order list

### API URL

    POST   /v2/order/list

**Parameter**

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| -----------------:|
| page    | int  |  yes   | current page   |
| page_size    | int  |  no   | page size   |

**Response**

| parameter           | type          | description             |
| ----------- |:----------:|:-----------:|
| code | integer|   0, -1 success, fail|
| msg  | string | success |
| data | array |  array or empty array |
| -cur_page  | integer |  current page |
| -page_size | integer |  page size |
| -total_page| integer |  total page |
| -total_num | integer |  total order number |
| -order_list| array |  order list |
| --order_id | integer |  order id |
| --order_status | integer |  order status |
| --created_at | datetime |  order purchase time |
| --updated_at | datetime |  order update time |
| --currency   | string   |  order currency |
| --price      | double   |  order price |
| --product_list | array |  product list |
| ---product_id | integer |  product id |
| ---product_name | string |  product name |
| ---product_status | integer |  order product status |
| ---product_line   | string | product line |
| ---departure_date  | date |   order departure date |
| ---end_date        | date |   order end date |
| ---rooms              | array   |  room info|
| ----adult            | integer |  adult number |
| ----kid              | integer |  kid number |
| ----single_pairup    | integer |  single pairup |
| ---price_info    | array |  price info |
| ----total_retail         | double |  total price |
| ----total_retail_target_currency | double |  target currency total retail|
| ----original_total_retail        | double | original total retail |
| ----original_total_retail_target_currency | double |  target currency origin total retail |
| ----total_discount       | double |  total discount |
| ----total_discount_target_currency        | double |  target currency discount price |
| ---contact          | array     |  contact info|
| ----first_name      | string   |  first name|
| ----last_name       | string   |  last name|
| ----mobile          | string   |  mobile|
| ----email           | string   |  email|

**Reqeust parameter example**
```
{
    "page":1
    "page_size" : 15 // default 10
}
```

**Response**
```
{
    "code": 0,
    "msg": "success",
    "data": {
        "cur_page": 1,
        "page_size": 10,
        "total_page": 2,
        "total_num": 11,
        "order_list": [
            {
                "order_id": 10001316,
                "created_at": "2017-04-27 10:41:05",
                "updated_at": "2017-08-22 15:29:41",
                "currency": "USD",
                "price": 0.0039,
                "product_list": [
                    {
                        "product_id": 101470392,
                        "product_name": "(6 days) Italy Venice + Florence + Rome + Vatican + Pisa + Milan Cultural In-depth Tour • Bridge of Sighs, Cathedral of Santa Maria del Fiore, Trevi Fountain, Colosseum, Frankfurt/Ulm/Essen Round Trip",
                        "product_status": 60030,
                        "product_line": "tour",
                        "departure_date": "2017-05-22",
                        "end_date": "2017-05-27",
                        "rooms": [
                            {
                                "adult": 2,
                                "kid": 0
                            }
                        ],
                        "price_info": {
                            "total_retail": 0,
                            "total_retail_target_currency": 0,
                            "original_total_retail": 0,
                            "original_total_retail_target_currency": 0,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
                        },
                        "contact": {}
                    }
                ]
            },
            {
                "order_id": 10001318,
                "created_at": "2017-04-27 11:05:01",
                "updated_at": "2017-08-22 15:29:40",
                "currency": "USD",
                "price": 0.0039,
                "product_list": [
                    {
                        "product_id": 101470392,
                        "product_name": "(6 days) Italy Venice + Florence + Rome + Vatican + Pisa + Milan Cultural In-depth Tour • Bridge of Sighs, Cathedral of Santa Maria del Fiore, Trevi Fountain, Colosseum, Frankfurt/Ulm/Essen Round Trip",
                        "product_status": 60030,
                        "product_line": "tour",
                        "departure_date": "2017-05-22",
                        "end_date": "2017-05-27",
                        "rooms": [
                            {
                                "adult": 2,
                                "kid": 0
                            }
                        ],
                        "price_info": {
                            "total_retail": 0,
                            "total_retail_target_currency": 0,
                            "original_total_retail": 0,
                            "original_total_retail_target_currency": 0,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
                        },
                        "contact": {}
                    }
                ]
            },
            {
                "order_id": 10001322,
                "created_at": "2017-04-27 11:10:46",
                "updated_at": "2017-08-22 15:29:39",
                "currency": "USD",
                "price": 0.0039,
                "product_list": [
                    {
                        "product_id": 101470392,
                        "product_name": "(6 days) Italy Venice + Florence + Rome + Vatican + Pisa + Milan Cultural In-depth Tour • Bridge of Sighs, Cathedral of Santa Maria del Fiore, Trevi Fountain, Colosseum, Frankfurt/Ulm/Essen Round Trip",
                        "product_status": 60030,
                        "product_line": "tour",
                        "departure_date": "2017-05-22",
                        "end_date": "2017-05-27",
                        "rooms": [
                            {
                                "adult": 2,
                                "kid": 0
                            }
                        ],
                        "price_info": {
                            "total_retail": 0,
                            "total_retail_target_currency": 0,
                            "original_total_retail": 0,
                            "original_total_retail_target_currency": 0,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
                        },
                        "contact": {}
                    }
                ]
            },
            {
                "order_id": 10003997,
                "created_at": "2019-01-16 19:42:48",
                "updated_at": "2019-01-16 19:42:50",
                "currency": "USD",
                "price": 1496.5068,
                "product_list": [
                    {
                        "product_id": 101457594,
                        "product_name": "[weff's annual hits] (4 days) in-depth tour of Los Angeles and themed projects: choose three of the eight themed projects",
                        "product_status": 10000,
                        "product_line": "tour",
                        "departure_date": "2019-01-20",
                        "end_date": "2019-01-23",
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
                        "contact": {
                            "firstname": "a",
                            "lastname": "b",
                            "telephone": "1",
                            "email": "2@q.q"
                        }
                    }
                ]
            }
        ]
    }
}
```
