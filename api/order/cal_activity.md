# 价格计算(一日游产品)

**[一日游产品](./cal_activity.md)**

[多日游产品](./cal_tour.md)

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
	      "product_line": "activity",       //产品线
	      "product_base_price": 3,     //产品基本费用
	      "product_upgrade_price": 5,  //产品升级项费用
	      "product_price": 8               //产品总价
	    }
	  }
	}