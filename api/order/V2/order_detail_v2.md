# 订单详情

**描述**

根据订单号，获取订单详情信息

### API地址

    POST   /v2/order/detail
	
**参数**

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| -----------------:|
| order_id    | integer  |  是   | 订单ID   |

**返回**

| 参数           | 类型          | 描述             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 成功, 失败| 
| msg  | string | success |
| data | array |  数组或空数组 |
| -order_id | integer |  订单ID |
| -order_status | integer |  订单状态 |
| -created_at | datetime |  创建时间 |
| -updated_at | datetime |  更新时间 |
| -price      | double   |  订单总价 |
| -product_list | array |  产品数组 |
| ---product_id | integer |  产品ID |
| ---product_name | string |  产品名字 |
| ---product_status | integer |  订单产品状态 |
| ---product_line   | string |  产品线 |
| ---departure_date  | date |   出团日期 |
| ---end_date        | date |   回团日期 |
| ---departure_address | string | 出发地点 |
| ---rooms              | array   |  （非票务产品参数）房间信息（含，成人数，儿童数，是否单人配方）|
| ----adult            | integer |  成人数量 |
| ----kid              | integer |  儿童数量 |
| ----single_pairup    | integer |  是否单人配房 |
| ---price_info    | array |  价格信息 |
| ----total_retail         | double |  总价 |
| ----total_retail_target_currency | double |  目标币种总价 |
| ----original_total_retail        | double |  产品原始总价 |
| ----original_total_retail_target_currency | double |  目标比重原始总价 |
| ----total_discount       | double |  总优惠价格 |
| ----total_discount_target_currency        | double |  目标币种总优惠价格 |
| ---contact          | array     |  联系人信息|
| ----first_name      | string   |  名|
| ----last_name       | string   |  姓|
| ----mobile          | string   |  电话|
| ----email           | string   |  邮箱|
| ---guest            | string   |  出行人信息（此参数根据产品获取的PassengerForm变化而不同）|
| ---upgrades         | string   |  升级项信息 |
| ----upgrade_id      | integer   |  升级项ID|
| ----option_id       | integer   |  升级项子选项ID|
| ----name            | string   |  升级项名称|
| ----subname         | string   |  升级项子名称|
| ----option_name         | string   |  升级项选项名称|
| ----provider_tour_code  | string   |  供应商tour code|
	
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
