# 价格计算

### 描述
根据用户选项，计算订单的价格。

### API地址

	/v1/order/cal
	
### 参数

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
		"rooms":[		//房间信息
			{
				"adult":2,
				"kid":0
			}
		],
		"tickets":{ // 票务信息 ticket only , sku_id : number
        	"12":3
        }
	}
	
### 返回示例

	{
	  "code": 0,
	  "msg": "",
	  "data": {
	    "retail": 11.63,    //总价  
	    "currency": "USD",  //币种
	    "product": {
	      "product_id": 9847,
	      "product_currency": "CNY",
	      "product_line": "activity",       //产品线
	      "product_base_price": 30,     //产品基本费用
	      "product_upgrade_price": 50,  //产品升级项费用
	      "product_price": 80               //产品总价
	    }
	  }
	}