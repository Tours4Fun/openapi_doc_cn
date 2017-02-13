# 创建订单(多日游产品)

[一日游产品](./add_order_activity.md)

**[多日游产品](./add_order_tour.md)**

### 描述

todo

### API地址

	/v1/order/add
	
### 参数

	{
	    "product_id":9847,  //产品id
	    "departure_date":"2017-02-22", //出发日期
	    "departure_address":"jhjhj",    //出发地点
	    "upgrades":{        //升级项
	        "43":["203"],
	        "30002":["30113"]
	    },
	    "rooms":[       //房间信息
	        {
				"adult":2,
				"kid":0
			},//房间1
			{
				"adult":1,
				"kid":0
			}//房间2	    ],
	    "contact":{     //联系人信息
	        "first_name":"a",
	        "last_name":"b",
	        "mobile":"1",
	        "email":"2@q.q"
	    },
	    "guest_info":[      //出行人信息
	        {
	            "type":"adult",
	            "firstname_en":"ghghg",
	            "mobile":"86-6767"
	        },
	        {
	            "type":"kid",
	            "firstname_en":"oooo",
	            "mobile":"86-67887"
	        }
	    ]
	
	}
	
### 返回示例

	{
	  "code": 0,
	  "msg": "",
	  "data": {
	    "order_id": 1694
	  }
	}