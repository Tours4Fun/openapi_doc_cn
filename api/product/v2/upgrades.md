# 产品升级项

### 描述

根据`产品号`、`出行日期`、`购买日期` 获取产品升级项列表


### API地址

    /v2/product/upgrades

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  是   | 产品ID号  |
| departure_date     | date  |  是   | 出行日期(Y-m-d)  |
| purchase_date     | date  |  否   | 购买日期(Y-m-d)默认服务器当前日期  |
| currency     | string  |  否   | 货币类型默认'USD'  |


### 参数实例

	{
    	"product_id" : 101457621,
    	"departure_date":"2018-01-12",
    	"currency" : "CNY"
    }



### 返回示例

	{
        "code": 0,
        "msg": "success",
        "data": [
            {
                //升级项目id
                "upgrade_id": 4,
                //升级项目名称
                "name": "机场接机",
                //子标题
                "sub_name": "",
                //货币类型
                "currency": "CNY",
                //提示
                "tips": "",
                //是否多选
                "can_multi_select": 0,
                //当can_multi_select为1时，此处表示需要选择的个数（ 0表示可以不选 ）；当can_multi_select为0时，这个选项无效，表示为必选项目
                "required": 1,
                //升级项目选项
                "options": [
                    {
                        //选项id
                        "option_id": 78,
                        //选项名称
                        "name": "如人数更多则需要报价",
                        "is_per_order": 0,
                        //提示
                        "tips": "",
                        //价格
                        "value": [
                            {
                                "name": "single",
                                "price": 0
                            },
                            {
                                "name": "double",
                                "price": 0
                            },
                            {
                                "name": "triple",
                                "price": 0
                            },
                            {
                                "name": "quad",
                                "price": 0
                            },
                            {
                                "name": "kid",
                                "price": 0
                            }
                        ]
                    },
                    {
                        "option_id": 93,
                        "name": "1个人 10:01pm-12:00am",
                        "is_per_order": 0,
                        "tips": "",
                        "value": [
                            {
                                "name": "prefix",
                                "price": 424.0145
                            }
                        ]
                    },
                    {
                        "option_id": 94,
                        "name": "2个人 10:01pm-12:00am",
                        "is_per_order": 0,
                        "tips": "",
                        "value": [
                            {
                                "name": "single",
                                "price": 0
                            },
                            {
                                "name": "double",
                                "price": 0
                            },
                            {
                                "name": "triple",
                                "price": 0
                            },
                            {
                                "name": "quad",
                                "price": 0
                            },
                            {
                                "name": "kid",
                                "price": 0
                            }
                        ]
                    },
                    {
                        "option_id": 95,
                        "name": "3个人 10:01pm-12:00am",
                        "is_per_order": 0,
                        "tips": "",
                        "value": [
                            {
                                "name": "single",
                                "price": 0
                            },
                            {
                                "name": "double",
                                "price": 0
                            },
                            {
                                "name": "triple",
                                "price": 0
                            },
                            {
                                "name": "quad",
                                "price": 0
                            },
                            {
                                "name": "kid",
                                "price": 0
                            }
                        ]
                    },
                    {
                        "option_id": 96,
                        "name": "4个人 10:01pm-12:00am",
                        "is_per_order": 0,
                        "tips": "",
                        "value": [
                            {
                                "name": "prefix",
                                "price": 130.466
                            }
                        ]
                    },
                    {
                        "option_id": 97,
                        "name": "5个人 10:01pm-12:00am",
                        "is_per_order": 0,
                        "tips": "",
                        "value": [
                            {
                                "name": "prefix",
                                "price": 110.8961
                            }
                        ]
                    },
                    {
                        "option_id": 98,
                        "name": "6个人 10:01pm-12:00am",
                        "is_per_order": 0,
                        "tips": "",
                        "value": [
                            {
                                "name": "single",
                                "price": 0
                            },
                            {
                                "name": "double",
                                "price": 0
                            },
                            {
                                "name": "triple",
                                "price": 0
                            },
                            {
                                "name": "quad",
                                "price": 0
                            },
                            {
                                "name": "kid",
                                "price": 0
                            }
                        ]
                    }
                ]
            }
        ]
    }