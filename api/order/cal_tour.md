# 价格计算(多日游产品)

[一日游产品](./cal_activity.md)

**[多日游产品](./cal_tour.md)**

### 描述
根据用户选项，计算订单的价格。

### API地址

	/v1/order/cal
	
### 参数

	{
		"product_id":100009369,  //产品id
		"departure_date":"2017-02-22", //出发日期
		"departure_address":"jhjhj",	//出发地点
		"upgrades":{		//升级项
			"149":["1444","1445"],
			"148":["1440"],
			"150":["1448"]
		},
		"rooms":[		//房间信息
			{
				"adult":2,
				"kid":0
			},//房间1
			{
				"adult":1,
				"kid":0
			}//房间2
		]
	}
	
### 返回示例

	{
	  "code": 0,
	  "msg": "",
	  "data": {
	    "retail": 798.4,    //总价  
	    "currency": "USD",  //币种
	    "product": {
	      "product_id": 100009369,
	      "product_line": "tour",       //产品线
	      "product_base_price": 626.4,     //产品基本费用
	      "product_upgrade_price": 172,  //产品升级项费用
	      "upgrades": [
	        {
	          "name": "第二天行程选择",
	          "price": [
	            {
	              "total": 38,
	              "name": "A-西点军校-名牌购物中心 "
	            },
	            {
	              "total": 34,
	              "name": "B-纽约自由行"
	            }
	          ]
	        },
	        {
	          "name": "机场",
	          "price": [
	            {
	              "total": 40,
	              "name": "4个人(11:01pm-8:59am)"
	            }
	          ]
	        },
	        {
	          "name": "做测试用",
	          "price": [
	            {
	              "total": 60,
	              "name": "测试2"
	            }
	          ]
	        }
	      ],
	      "product_price": 798.4               //产品总价
	    }
	  }
	}