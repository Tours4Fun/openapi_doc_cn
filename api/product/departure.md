# 产品出发地点

### 描述

根据`产品号`、`日期` 获取产品出发地点


### API地址

    /v1/product/departure

### 参数

	{
		"product_id":100009369,
		"date":"2017-1-24"
	}



### 返回示例

	{
	  "code": 0,
	  "msg": "success",
	  "data": [
	    {
	      "id": 1528,
	      "time": "04:00:00",
	      "location": "LGA机场",
	      "address": "LGA机场",
	      "tips": "32142"
	    }
	  ]
	}

