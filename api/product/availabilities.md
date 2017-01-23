# 产品可售日期

### 描述

根据`产品号` 获取产品可售日期列表


### API地址

    /v1/product/availabilities

### 参数

	{
		"product_id":100009369
	}



### 返回示例

	{
	  "code": 0,
	  "msg": "",
	  "data": {
	    "currency": "CNY",
	    "availabilities": [
	      {
	        "date": "2017-01-24",
	        "display_price": "99.9800",
	        "min_persons": 1
	      },
	      {
	        "date": "2017-01-25",
	        "display_price": "99.9800",
	        "min_persons": 1
	      },
	      {
	        "date": "2017-01-31",
	        "display_price": "99.9800",
	        "min_persons": 1
	      },
	      {
	        "date": "2017-02-01",
	        "display_price": "99.9800",
	        "min_persons": 1
	      }
	    ]
	  }
	}


