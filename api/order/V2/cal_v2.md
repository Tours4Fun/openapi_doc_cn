# 价格计算

**描述**

根据用户选项，计算订单的价格。

### API地址

    POST   /v2/order/cal

**参数**

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| -----------------:|
| product_id    | int  |  是   | 产品ID   |
| adult         | int  |  是   | 成人数量 |
| kid           | int |  是    | 小孩数量 |
| departure_date      | string  |  是   |  出团日期|
| departure_address   |string   |  是   | 出发地点|
| upgrades            | array   |  是   | 升级项（升级项ID：升级项子项ID）|
| rooms               | array   |  是   | 房间信息（含，成人数，儿童数，是否单人配方）|

**请求参数示例**

（以下请求参数适用于一日游，多日游产品线）
```
    {
        "product_id":102202692, 
        "adult":2,  
        "kid":0,        
        "departure_date":"2019-01-16", 
        "departure_address":"jhjhj",    
        "upgrades":{       
            "30100":["30577"]
        },
        "rooms":[       
            {
                "adult":2,
                "kid":0
            }
        ]
    }
```
（以下参数适用于票务产品线）
```
    {
		"product_id":9847,  //产品id
		"adult":1,	//成人数量
		"kid":1,		//小孩数量
		"departure_date":"2017-02-22", //出发日期
		"departure_address":"jhjhj",	//出发地点
		"upgrades":{		//升级项
			"43":["203"],
			"30002":["30113"]
		},
		"tickets":[ // 票务信息 ticket only , sku_id : count
        	{
               "sku_id":15021,
               "count":1
            }
        ]
	}
```
**结果返回示例**

 一日游，多日游返回示例
```
{
        "product_id" => 102202692
          "product_line" => "activity"
          "currency" => "EUR"
          "total_retail" => 61.6
          "total_retail_target_currency" => 71.728
          "original_total_retail" => 80
          "original_total_retail_target_currency" => 93.1532
          "total_discount" => 18.4
          "total_discount_target_currency" => 21.4252
          "product_price_detail" => array:2 [
            "base_price" => array:3 [
              "total_retail" => 61.6
              "original_total_retail" => 80
              "base_price_detail" => array:1 [
                0 => array:4 [
                  "total_retail" => 61.6
                  "total_retail_target_currency" => 71.728
                  "original_total_retail" => 80
                  "original_total_retail_target_currency" => 93.1532
                ]
              ]
            ]
            "upgrades_price" => array:3 [
              "total_retail" => 0
              "total_retail_target_currency" => 0
              "upgrades_detail" => array:1 [
                30100 => array:4 [
                  "total_retail" => 0
                  "total_retail_target_currency" => 0
                  "upgrade_name" => "座位等级"
                  "upgrades_sub_detail" => array:1 [
                    0 => array:4 [
                      "option_id" => 30577
                      "total_retail" => 0
                      "total_retail_target_currency" => 0
                      "upgrade_sub_name" => "一等(First Class-Max.2 passengers)"
                    ]
                  ]
                ]
              ]
            ]
          ]
}
```
票务产品返回示例
```
{
     "product_id" => 102202730
      "product_line" => "ticket"
      "currency" => "CAD"
      "total_retail" => 77.75
      "total_retail_target_currency" => 59.7617
      "original_total_retail" => 77.75
      "original_total_retail_target_currency" => 59.7617
      "total_discount" => 0
      "total_discount_target_currency" => 0
      "product_price_detail" => array:2 [
        "base_price" => array:5 [
          "total_retail" => 77.75
          "total_retail_target_currency" => 59.7617
          "original_total_retail" => 77.75
          "original_total_retail_target_currency" => 59.7617
          "base_price_detail" => array:1 [
            0 => array:6 [
              "total_retail" => 77.75
              "total_retail_target_currency" => 59.7617
              "original_total_retail" => 77.75
              "original_total_retail_target_currency" => 59.7617
              "sku_id" => 15021
              "sku_name" => "生态游船观海豚-成人"
            ]
          ]
        ]
        "upgrades_price" => array:3 [
          "total_retail" => 0
          "total_retail_target_currency" => 0
          "upgrades_detail" => array:2 [
            219 => array:4 [
              "total_retail" => 0
              "total_retail_target_currency" => 0
              "upgrade_name" => "游船出发时间选择(请以供应商最终确认为准)"
              "upgrades_sub_detail" => array:1 [
                0 => array:4 [
                  "option_id" => 1375
                  "total_retail" => 0
                  "total_retail_target_currency" => 0
                  "upgrade_sub_name" => "08:45珀斯市区码头出发"
                ]
              ]
            ]
            221 => array:4 [
              "total_retail" => 0
              "total_retail_target_currency" => 0
              "upgrade_name" => "用餐时间"
              "upgrades_sub_detail" => array:1 [
                0 => array:4 [
                  "option_id" => 1378
                  "total_retail" => 0
                  "total_retail_target_currency" => 0
                  "upgrade_sub_name" => "12:00"
                ]
              ]
            ]
          ]
        ]
      ]
}
```