# 产品升级项

### 描述

根据`产品号`、`日期` 获取产品升级项列表


### API地址

    /v1/product/upgrades

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
	      "option_id": 148,
	      "name": "机场",
	      "tips": "机场接送",
	      "can_multi_select": 1,
	      "value": [
	        {
	          "value_id": 1435,
	          "name": "9:00am-11:00pm 免费"
	        },
	        {
	          "value_id": 1436,
	          "name": "如需更多请联系我们取得报价"
	        },
	        {
	          "value_id": 1437,
	          "name": "1个人(11:01pm-8:59am)"
	        }
	      ]
	    },
	    {
	      "option_id": 149,
	      "name": "第二天行程选择",
	      "tips": "",
	      "can_multi_select": 1,
	      "value": [
	        {
	          "value_id": 1444,
	          "name": "A-西点军校-名牌购物中心 "
	        },
	        {
	          "value_id": 1445,
	          "name": "B-纽约自由行"
	        },
	        {
	          "value_id": 1446,
	          "name": "C-纽约-大西洋赌城-纽约(限21岁以上) "
	        }
	      ]
	    }
	  ]
	}