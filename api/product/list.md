# 产品列表

### 描述

根据`地区`、`产品线` 获取产品列表


### API地址

    /v1/product/list

### 参数

	{
		"region":"美国", // 地区 ，非必填
		"product_line":"activity", //activity or tour ，非必填
		"page":1 //默认1， 非必填
	}



### 返回示例

	{
	  "code": 0,
	  "msg": "success",
	  "data": {
	    "count": 0,
	    "page": "1",
	    "page_size": 20,
	    "products": [
	      {
	        "product_id": "13570",
	        "name": "[洛杉矶市区1日游] 好莱坞+比佛利山庄",
	        "image_url": "http://dn-toursforfun.qbox.me/images/201504271430119119_553de2cfd8b1d_watermark_800_800.jpg",
	        "product_line": "activity",
	        "duration": "1.00",
	        "duration_type": "day",
	        "sub_region": "east",
	        "sub_region_chinese_name": "美东",
	        "region": "us",
	        "region_chinese_name": "美国",
	        "advertised_price": "33.000000",
	        "departure_city": [
	          "纽约"
	        ],
	        "return_city": [
	          "纽约"
	        ],
	        "visited_city": [
	          "洛杉矶",
	          "圣塔莫尼卡",
	          "纽约",
	          "梦幻世界"
	        ]
	      }
	    ]
	  }
	}


