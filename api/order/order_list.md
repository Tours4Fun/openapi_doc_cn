# 订单列表

### 描述

获取当前应用下的订单列表

### API地址

	/v1/order/list
	
### 参数

	{
	    "page":1  //页码
	}
	
### 返回示例

	{
	    "code":0,
	    "msg":"",
	    "data":{
	        "cur_page":1,       //当前页码
	        "page_size":10,     //每页数量
	        "total_page":30,    //总页数
	        "total_num":294,    //总订单数
	        "order_list":[      //订单列表
	            {
	                "order_id":1409,        //订单号
	                "status":100,           //状态
	                "created_at":"2016-11-30 14:30:54",
	                "updated_at":"2016-11-30 14:30:54",
	                "currency":"USD",
	                "price":28.67,
	                "product_list":[        //产品信息
	                    {
	                        "product_id":100020977,
	                        "product_name":"(SYNC 1107) Panda Show, Las Vegas (熊猫秀)[clone]",
	                        "product_line":"ticket",
	                        "departure_date":"2016-11-28",
	                        "rooms":"room_info",
	                        "price_info":{
	                            "product_price": "21.50",
					              "upgrades_price": "7.17",
					              "final_price": 28.67
	                        },
	                        "contact":{
	                            "firstname":"Blues",
	                            "lastname":"Ram",
	                            "mobile":"86-18688124774",
	                            "email":"admin@lanhao.name"
	                        }，
	                        "guest": [
						          {
						            "order_product_guest_id": 2509,
						            "order_product_id": 1374,
						            "telephone": null,
						            "email": null,
						            "passport_no": null,
						            "type": "adult",
						            "firstname_en": "ghghg",
						            "mobile": "86-6767"
						          },
						          {
						            "order_product_guest_id": 2510,
						            "order_product_id": 1374,
						            "telephone": null,
						            "email": null,
						            "passport_no": null,
						            "type": "kid",
						            "firstname_en": "oooo",
						            "mobile": "86-67887"
						          }
						        ],
						        "upgrades": [
						          {
						            "upgrade": "主题公园<font color=#f0000f>(下单时请备注您需要的语种)</font>",
						            "value": "迪士尼乐园aa"
						          },
						          {
						            "upgrade": "洛杉矶酒店升级",
						            "value": "Best Western Executive,Rowland Heights(罗兰岗最佳西方集团酒店)-Freeway Side"
						          }
						        ]
	                    }
	                ]
	            }
	        ]
	    }
	}