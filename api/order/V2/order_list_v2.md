# 订单列表

**描述**

根据页数，获取订单列表信息

### API地址

    POST   /v2/order/list
	
**参数**

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| -----------------:|
| page    | int  |  是   | 当前页数   |
| page_size    | int  |  否   | 页面偏移量   |

**返回**

| 参数           | 类型          | 描述             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 成功, 失败| 
| msg  | string | success |
| data | string |  array |
	
**请求参数示例**
```
{
    "page":1  //页码
    "page_size" : 15 //页面偏移量， 不传则默认为10
}
```

**返回示例**
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
                        "product_name": "(6天)意大利威尼斯+佛罗伦萨+罗马+梵蒂冈+比萨+米兰人文深度游 • 叹息桥、圣母百花大教堂、许愿池、罗马斗兽场、法兰克福/乌尔姆/埃森往返",
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
                        "product_name": "(6天)意大利威尼斯+佛罗伦萨+罗马+梵蒂冈+比萨+米兰人文深度游 • 叹息桥、圣母百花大教堂、许愿池、罗马斗兽场、法兰克福/乌尔姆/埃森往返",
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
                        "product_name": "(6天)意大利威尼斯+佛罗伦萨+罗马+梵蒂冈+比萨+米兰人文深度游 • 叹息桥、圣母百花大教堂、许愿池、罗马斗兽场、法兰克福/乌尔姆/埃森往返",
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
                "order_id": 10003122,
                "created_at": "2018-07-29 16:43:19",
                "updated_at": "2018-07-29 16:43:20",
                "currency": "USD",
                "price": 80.0879,
                "product_list": [
                    {
                        "product_id": 102202270,
                        "product_name": "票务123",
                        "product_status": 10000,
                        "product_line": "ticket",
                        "departure_date": "2018-03-07",
                        "end_date": "2018-03-07",
                        "rooms": [
                            {
                                "adult": 1,
                                "child": 0
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
                        "contact": {
                            "firstname": "",
                            "lastname": "mafengwo",
                            "telephone": "028-85540555",
                            "email": "mfworders@toursforfun.com"
                        }
                    }
                ]
            },
            {
                "order_id": 10003996,
                "created_at": "2019-01-16 19:39:03",
                "updated_at": "2019-01-16 19:39:05",
                "currency": "USD",
                "price": 71.728,
                "product_list": [
                    {
                        "product_id": 102202692,
                        "product_name": "【都市之旅】纽约一日游·自由女神像+帝国大厦+无畏号航舰博物馆[clone]",
                        "product_status": 10000,
                        "product_line": "activity",
                        "departure_date": "2019-01-16",
                        "end_date": "2019-01-16",
                        "rooms": [
                            {
                                "adult": 2,
                                "kid": 0,
                                "single_pairup": 1
                            }
                        ],
                        "price_info": {
                            "total_retail": 61.6,
                            "total_retail_target_currency": 71.728,
                            "original_total_retail": 80,
                            "original_total_retail_target_currency": 93.1532,
                            "total_discount": 18.4,
                            "total_discount_target_currency": 21.4252
                        },
                        "contact": {
                            "firstname": "a",
                            "lastname": "b",
                            "telephone": "1",
                            "email": "2@q.q"
                        }
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
                        "product_name": "【weff年度爆品】(4天)洛杉矶、主题项目深度游：八大主题项目任选三",
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
            },
            {
                "order_id": 10003998,
                "created_at": "2019-01-16 19:44:06",
                "updated_at": "2019-01-16 19:44:08",
                "currency": "USD",
                "price": 59.7617,
                "product_list": [
                    {
                        "product_id": 102202730,
                        "product_name": "杰维斯湾游船看海豚生态观光之旅Jervis Bay Dolphin Eco Tour(午餐可选)",
                        "product_status": 10000,
                        "product_line": "ticket",
                        "departure_date": "2019-01-16",
                        "end_date": "2019-01-16",
                        "rooms": [],
                        "price_info": {
                            "total_retail": 77.75,
                            "total_retail_target_currency": 59.7617,
                            "original_total_retail": 77.75,
                            "original_total_retail_target_currency": 59.7617,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
                        },
                        "contact": {
                            "firstname": "a",
                            "lastname": "b",
                            "telephone": "1",
                            "email": "2@q.q"
                        }
                    }
                ]
            },
            {
                "order_id": 10003999,
                "created_at": "2019-01-16 19:45:02",
                "updated_at": "2019-01-16 19:45:04",
                "currency": "USD",
                "price": 393.5724,
                "product_list": [
                    {
                        "product_id": 102202254,
                        "product_name": "新增测试酒店sync6666",
                        "product_status": 10000,
                        "product_line": "hotel",
                        "departure_date": "2019-01-16 3:00:00",
                        "end_date": "2019-01-16 3:00:00",
                        "rooms": [
                            {
                                "hotel_room_id": 14838568,
                                "adult": 1,
                                "kid": 0,
                                "ages": "",
                                "special_note": "",
                                "firstname_en": "ghghg",
                                "lastname_en": ""
                            }
                        ],
                        "price_info": {
                            "total_retail": 338,
                            "total_retail_target_currency": 393.5724,
                            "original_total_retail": 338,
                            "original_total_retail_target_currency": 393.5724,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
                        },
                        "contact": {
                            "firstname": "a",
                            "lastname": "b",
                            "telephone": "1",
                            "email": "2@q.q"
                        }
                    }
                ]
            },
            {
                "order_id": 10004000,
                "created_at": "2019-01-16 19:45:55",
                "updated_at": "2019-01-16 19:45:57",
                "currency": "USD",
                "price": 196.7862,
                "product_list": [
                    {
                        "product_id": 102202254,
                        "product_name": "新增测试酒店sync6666",
                        "product_status": 10000,
                        "product_line": "hotel",
                        "departure_date": "2019-01-17 3:00:00",
                        "end_date": "2019-01-17 3:00:00",
                        "rooms": [
                            {
                                "hotel_room_id": 14838568,
                                "adult": 1,
                                "kid": 0,
                                "ages": "",
                                "special_note": "",
                                "firstname_en": "ghghg",
                                "lastname_en": ""
                            }
                        ],
                        "price_info": {
                            "total_retail": 169,
                            "total_retail_target_currency": 196.7862,
                            "original_total_retail": 169,
                            "original_total_retail_target_currency": 196.7862,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
                        },
                        "contact": {
                            "firstname": "a",
                            "lastname": "b",
                            "telephone": "1",
                            "email": "2@q.q"
                        }
                    }
                ]
            },
            {
                "order_id": 10004001,
                "created_at": "2019-01-17 09:39:44",
                "updated_at": "2019-01-17 09:39:46",
                "currency": "USD",
                "price": 196.7862,
                "product_list": [
                    {
                        "product_id": 102202254,
                        "product_name": "新增测试酒店sync6666",
                        "product_status": 10000,
                        "product_line": "hotel",
                        "departure_date": "2019-01-17 3:00:00",
                        "end_date": "2019-01-17 3:00:00",
                        "rooms": [
                            {
                                "hotel_room_id": 14838568,
                                "adult": 1,
                                "kid": 0,
                                "ages": "",
                                "special_note": "",
                                "firstname_en": "ghghg",
                                "lastname_en": ""
                            }
                        ],
                        "price_info": {
                            "total_retail": 169,
                            "total_retail_target_currency": 196.7862,
                            "original_total_retail": 169,
                            "original_total_retail_target_currency": 196.7862,
                            "total_discount": 0,
                            "total_discount_target_currency": 0
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