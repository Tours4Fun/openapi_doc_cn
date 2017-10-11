# 价格计算(一日游产品)

**[一日游产品](./cal_activity.md)**

[多日游产品](./cal_tour.md)

### 描述
根据用户选项，计算订单的价格。

### API地址

	/v1/order/cal
	
### 参数

	{
		"product_id":13374,  //产品id
		"adult":1,	//成人数量
		"kid":1,		//小孩数量
		"departure_date":"2017-05-04", //出发日期
		"departure_address":"jhjhj",	//出发地点
		"upgrades":{		//升级项
			"4":["93"],
			"30002":["30116"]
		}
	}
	
### 返回示例

	{
	  "code": 0,
	  "msg": "success",
	  "data": {
	    "retail": 295,
	    "currency": "USD",
	    "product": {
	      "product_id": 13374,
	      "product_line": "activity",
	      "product_base_price": "265.00",
	      "product_upgrade_price": "30.00",
	      "upgrades": [  //升級項價格明細
	        {
	          "upgrade_id": 4,
	          "option_id": 93,
	          "price": 30
	        },
	        {
	          "upgrade_id": 30002,
	          "option_id": 30116,
	          "price": 0
	        }
	      ],
	      "base_price": {
                "adult_num": 1,
                "kid_num": 1,
                "single_adult_price": 170,
                "single_kid_price": 125,
                "total_adult_price": 170,
                "total_kid_price": 125
              },
	      "product_price": 295
	    }
	  }
	}
