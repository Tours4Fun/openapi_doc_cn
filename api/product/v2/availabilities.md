# 产品可售日期

### 描述

根据`产品号` 获取产品可售日期列表,


**确定返回天数**
### API地址

    /v2/product/availabilities

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  是   | 产品ID号  |

### 参数实例
    
    {
    	"product_id":101686926
    }

### 返回示例

    一日游：
	{
        "code": 0,
        "msg": "success",
        "data": {
            //货币类型
            "currency": "CNY",
            //货币符号
            "symbol": "¥",
            "price": {
                //成人价格
                "adult": 80,
                //儿童价格
                "kid": 59
            },
            "availabilities": [
                {
                    //日期
                    "date": "2018-01-16",
                    //展示价格
                    "display_price": "406.16",
                    //最少预定人数
                    "min_persons": 2
                },
                {
                    "date": "2018-01-17",
                    "display_price": "406.16",
                    "min_persons": 2
                },
                {
                    "date": "2018-01-18",
                    "display_price": "406.16",
                    "min_persons": 2
                },
                {
                    "date": "2018-01-19",
                    "display_price": "406.16",
                    "min_persons": 2
                }
            ]
        }
    }
    
    多日游：
    {
        "code": 0,
        "msg": "success",
        "data": {
            "currency": "USD",
            "symbol": "$",
            "price": {
                //单人间价格
                "single": "1295.0000",
                //双人间价格
                "double": "881.0000",
                //三人间价格
                "triple": "797.0000",
                //四人间价格
                "quad": "755.0000",
                //小孩价格
                "kid": "631.0000"
            },
            "availabilities": [
                {
                    "date": "2018-01-17",
                    "display_price": 325,
                    "min_persons": 1
                },
                {
                    "date": "2018-01-22",
                    "display_price": 325,
                    "min_persons": 1
                }
            ]
        }
    }
	

