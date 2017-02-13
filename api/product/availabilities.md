# 产品可售日期

### 描述

根据`产品号` 获取产品可售日期列表,

价格部分统一只返回 `USD`

**确定返回天数**
### API地址

    /v1/product/availabilities

### 参数

	{
		"product_id":100009369
	}



### 返回示例

	{
	  "code": 0,
	  "msg": "success",
	  "data": {
	    "currency": "USD",
	    "availabilities": [
	      {
	        "date": "2017-01-24",
	        "display_price": "394.00",
	        "min_persons": 1
	      },
	      {
	        "date": "2017-01-25",
	        "display_price": "394.00",
	        "min_persons": 1
	      },
	      {
	        "date": "2017-01-26",
	        "display_price": "394.00",
	        "min_persons": 1
	      }
	    ]
	  }
	}
	

