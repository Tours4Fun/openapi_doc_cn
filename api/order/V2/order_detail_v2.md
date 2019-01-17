# 订单详情

**描述**

根据订单号，获取订单详情信息

### API地址

    POST   /v2/order/detail
	
**参数**

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| -----------------:|
| order_id    | int  |  是   | 订单ID   |

**返回**

| 参数           | 类型          | 描述             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 成功, 失败| 
| msg  | string | success |
| data | string |  array |
	
**请求参数示例**
```
    {
	    "order_id":1672
	}
```

**返回示例**
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
                "product_name": "【weff年度爆品】(4天)洛杉矶、主题项目深度游：八大主题项目任选三",
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
                        "name": "机场l接机",
                        "subname": "",
                        "option_name": "如人数更多则需要报价",
                        "provider_tour_code": ""
                    },
                    {
                        "upgrade_id": 9,
                        "option_id": 60,
                        "name": "酒店升级",
                        "subname": "",
                        "option_name": "Westin Bonaventure Downtown Los Angeles(洛杉矶博纳旺蒂尔威斯汀大酒店)(限08/01-12/31/13期间入住)(4星级)",
                        "provider_tour_code": ""
                    }
                ]
            }
        ]
    }
}
```
