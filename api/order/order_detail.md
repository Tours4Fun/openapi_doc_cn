# 订单详情

### 描述
根据订单号，获取订单详情信息

### API地址

	/v1/order/detail
	
### 参数

	{
	    "order_id":1672
	}
	
### 返回示例

	{
	  "code": 0,
	  "msg": "",
	  "data": {
	    "order_id": 1672,
	    "status": 100,
	    "created_at": "2017-01-17 16:34:39",
	    "updated_at": "2017-01-17 16:34:41",
	    "price": 28.67,
	    "product_list": [
	      {
	        "product_id": 9847,
	        "product_name": "33dddd舍大街,协和广场,埃菲尔铁塔,凡尔赛宫,卢浮宫舍大街,协和广场,埃菲尔铁塔,凡尔赛宫,卢浮宫\r\n布鲁塞尔出发,巴黎结束",
	        "product_line": "activity",
	        "departure_date": "2017-02-22",
	        "rooms": [
	          {
	            "adult": 2,
	            "kid": 0
	          }
	        ],
	        "price_info": {
	          "product_price": 21.5,
              "upgrades_price": 7.17,
              "final_price": 28.67
	        },
	        "contact": [
	          {
	            "firstname": "",
	            "lastname": "",
	            "mobile": "",
	            "email": "2@q.q"
	          }
	        ],
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
	}