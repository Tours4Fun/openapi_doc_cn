# Product Upgrades

### Description

Obtain a list of product upgrade items based on `product id`, `departure date`, `purchase date`


### API URL

    /v2/product/upgrades

### Parameter

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  yes   | product id  |
| departure_date     | date  |  yes   | departure date(Y-m-d)  |
| purchase_date     | date  |  no   | purchase date(Y-m-d), default current date |
| currency     | string  |  no   | default currency 'USD'  |


### Reqeust parameter example

	{
    	"product_id" : 101457621,
    	"departure_date":"2018-01-12",
    	"currency" : "CNY"
    }



### Response

	{
        "code": 0,
        "msg": "success",
        "data": [
            {
                //upgrade id
                "upgrade_id": 4,
                //upgrade name
                "name": "airport pickup",
                //upgrade sub name
                "sub_name": "",
                //currency
                "currency": "CNY",
                //upgrade tips
                "tips": "",
                "can_multi_select": 0,
                //when can_multi_select is 1, required means must select number of "required" corresponding values
                "required": 1,
                //upgrade options
                "options": [
                    {
                        "option_id": 78,
                        "name": "opiton A",
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
                        "option_id": 93,
                        "name": "one person 10:01pm-12:00am",
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
                        "name": "two person 10:01pm-12:00am",
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
                        "name": "three person 10:01pm-12:00am",
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
                        "name": "four person 10:01pm-12:00am",
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
                        "name": "five person 10:01pm-12:00am",
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
                        "name": "six person 10:01pm-12:00am",
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
