# 产品出发地点

### 描述

根据`产品号`、`出行日期` 获取产品出发地点


### API地址

    /v2/product/departure

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  是   | 产品ID号  |
| departure_date     | date  |  是   | 出行时间(Y-m-d)  |

### 参数实例

    {
    	"product_id" : 101457621,
    	"departure_date" : "2018-01-12"
    }

### 返回示例

	{
        "code": 0,
        "msg": "success",
        "data": [
            {
                //departure_id
                "id": 32903,
                //上车时间 如果只有start_time,代表一个时间点;start_time、end_time都存在代表一个时间段;如果start_time、end_time都为空代表不限时间
                "start_time": "11:00:00",
                "end_time": "",
                //地点
                "location": "12121",
                //地址
                "address": "12212112",
                //提示
                "tips": "12211222"
            },
            {
                "id": 32902,
                "start_time": "12:00:00",
                "end_time": "",
                "location": "Location",
                "address": "Full Address",
                "tips": "Tips\tTips"
            }
        ]
    }

