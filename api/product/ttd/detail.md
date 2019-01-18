# Product Detail Info

### Description

    Get the product Detail Info

### API address

    api_open/product/detail

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| productIds          | array         |     Yes     |   Product Ids[max:50]           |
| returnFields        | array         |     No      |   Optional Module:basic, info, departure, skuInfo, passengerForm, FinedPolicy[default:all modules]          |

### Request parameter demo

	{
    	"productIds":[102851680],
    	"returnFields":["basic", "info", "departure", "skuInfo","passengerForm","finedPolicy"]
    }

### Request parameter description

    basic
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| product_id                        |     Product Unique Id                             |
| product_type                      |     Product Type [See Table 1 For Details.]       |
| name                              |     Product Name                                  |
| departure_city                    |     Departure City                                |
| departure_city.id                 |     Id                                            |
| departure_city.name_en            |     English Name                                  |
| departure_city.name               |     Chinese Name                                  |
| return_city                       |     Return City                                   |
| return_city.id                    |     Id                                            |
| return_city.name_en               |     English Name                                  |
| return_city.name                  |     Chinese Name                                  |
| activity_type                     |     Type Of Activity                              |
| duration                          |     Product Duration                              |
| duration_type                     |     Product Duration Unit[min,hour,day]           |
| is_vega_show                      |     Show Ticket[0=>No, 1=>Yes]                    |
| product_region                     |     Type Of Activity                              |
| product_sub_region                     |     Type Of Activity                              |



### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "102851680": {
                "basic": {
                    "product_id": 102851680,
                    "product_type": 2,
                    "name": "Testing Alpesh product",
                    "departure_city": [
                        {
                            "city_id": 27697,
                            "name": "Vail",
                            "description": ""
                        }
                    ],
                    "return_city": [
                        {
                            "city_id": 30211,
                            "name": "Mill Valley",
                            "description": ""
                        }
                    ],
                    "activity_type": 0,
                    "ticket_type": 129,
                    "duration": 3,
                    "duration_type": "hour",
                    "is_vega_show": 0,
                    "product_region": 1,
                    "product_sub_region": 11,
                    "currency": "EUR",
                    "departure_location_status": 0,
                    "end_location_status": 3,
                    "language": [
                        {
                            "language_id": 46,
                            "name": "English Audio"
                        },
                        {
                            "language_id": 47,
                            "name": "English Live"
                        }
                    ],
                    "image_url": [
                        "http://img1.dev5.tff.com/f1/windtour/0f/9d/tiyan3.jpg",
                        "http://img1.dev5.tff.com/f1/windtour/37/46/qa-title.png"
                    ],
                    "video_url": ""
                },
                "info": {
                    "brief_description": "*途风和美国洛杉矶出团数量最大的巴士地接公司强强合作！*由洛杉矶最具经验的专职双语导游带您游览环球影城以及好莱坞，您将在这里领略到著名影视城的独特魅力。",
                    "summary": "Itinerary summery",
                    "notice": "【友情提示】* 如果您准备假日(新年/圣诞)期间外出旅行，请尽量提前一个月预订该团。* 如果您在出发前需要临时更改上车地点，请务必于出团日期前五天告知我们，以便我们进行协调安排；如果未提前五天进行告知，将不予更改，请您悉知，感谢您的理解及支持！",
                    "includes": "空调大巴或中巴免费地面接送(请参考接送时间和地点)",
                    "excludes": "不包括提供给导游和司机的服务费(每位客人支付司机及导游服务费：共$8.00/每天)",
                    "package_special_note": "温馨提示：该行程提供多个上车地点供您选择，在行程正式开始前，您可能会乘坐接应大巴从选择的上车点转移到集合中心，与其它上车点的客人汇合，给您带来不便敬请见谅！",
                    "price_special_note": "*成人：10岁或以上 *小孩： 3-9岁",
                    "eticket_special_note": "为确保您的行程顺利，请您在出发前一天务必致电给地接社或途风获取并确认领队的联络方式。",
                    "tips": "itinerary Tips",
                    "travel_notice": "",
                    "how_to_use": "eticket instructions: This is automatic generate e-ticket.",
                    "airport_transfer_info": "provider will provide the airport transfer info later.we will inform you for same.",
                    "contain_airport_transfer": 2,
                    "is_welcome_board": 1,
                    "flight_time_limit": 2,
                    "attractions": [
                        {
                            "city_id": 32299,
                            "name": "Kelly Ingram Park",
                            "description": ""
                        },
                        {
                            "city_id": 29197,
                            "name": "Sunset Crater Volcano National Monument",
                            "description": ""
                        }
                    ],
                    "cities": [
                        {
                            "city_id": 27697,
                            "name": "Vail",
                            "description": ""
                        },
                        {
                            "city_id": 29473,
                            "name": "德国村Leavenworth",
                            "description": "德国村位于西雅图东北部，约二个半小时车程的山区里，是处洋溢着德国巴伐利亚风情的山间城镇，也是西雅图近郊最受欢迎的观光小镇，无论是庆祝活动最多的夏天、枫红点点的秋天，还是挂满圣诞灯饰的银白冬天，这里的气氛随时都充满着欢乐，深受游客的喜爱。游客来到德国村，可以逛逛村里共90多家商店，商店里除了贩卖具代表性的德国工艺品，像是咕咕钟、胡桃钳娃娃，还有各式来自欧洲的精美工艺品，让人眼花缭乱。"
                        },
                        {
                            "city_id": 30211,
                            "name": "Mill Valley",
                            "description": ""
                        }
                    ],
                    "ownexpenses": [
                        {
                            "ownexpense_id": 2634,
                            "name": "波士顿美术博物馆",
                            "description": "收藏东方艺术品着称于世，现藏有中国和日本绘画5000余幅。其中有相当数量的宋、元时期名画，如保存完好的唐张萱《捣练图》，宋代摹本、宋徽宗《五色鹦鹉》等。其他绘画藏品也十分丰富，有格列柯、委拉斯贵兹、提香、丁托莱托、罗索等人的作品，有伦勃朗、鲁本斯、普桑、夏尔丹、库尔贝、马奈、德加、华托、雷诺阿、保罗•塞尚、梵•高的作品。",
                            "price": "成人$25.00/人；小孩(3-12岁)免费；老人(62岁以上)$25.00/人",
                            "duration": "",
                            "tips": ""
                        },
                        {
                            "ownexpense_id": 3843,
                            "name": "好莱坞环球影城一日游",
                            "description": "游览好莱坞星光大道、主题公园环球影城主题公园。",
                            "price": "成人$170.00/人；小孩(3-9岁)$165.00/人",
                            "duration": "",
                            "tips": ""
                        }
                    ]
                },
                "departure": {
                    "start_locations": {
                        "location_status": 0,
                        "locations": [
                            {
                                "departure_id": 155,
                                "start_time": "08:00:01",
                                "end_time": "09:00:01",
                                "region": "Los Angeles",
                                "location": "罗思密品质酒店(Quality Inn Rosemead)",
                                "address": "9488 Valley Blvd., Rosemead, CA 91770",
                                "tips": "温馨提示：请您在该酒店门口处等待接应巴士。",
                                "longitude": -118.062728,
                                "latitude": 34.0808498,
                                "operations": [
                                    {
                                        "start_date": "2018-12-01",
                                        "end_date": "2019-03-01",
                                        "sunday": 0,
                                        "monday": 1,
                                        "tuesday": 1,
                                        "wednesday": 1,
                                        "thursday": 1,
                                        "friday": 1,
                                        "saturday": 1
                                    }
                                ]
                            }
                        ]
                    },
                    "end_locations": {
                        "location_status": 3,
                        "locations": []
                    }
                },
                "passengerForm": [
                    {
                        "name": "firstname_en",
                        "type": "text",
                        "options": []
                    },
                    {
                        "name": "lastname_en",
                        "type": "text",
                        "options": []
                    },
                    {
                        "name": "passport",
                        "type": "text",
                        "options": []
                    },
                    {
                        "name": "passport_expire",
                        "type": "date",
                        "options": []
                    },
                    {
                        "name": "mobile",
                        "type": "phone",
                        "options": []
                    },
                    {
                        "name": "email",
                        "type": "text",
                        "options": []
                    },
                    {
                        "name": "gender",
                        "type": "radio",
                        "options": [
                            "未定义",
                            "男",
                            "女"
                        ]
                    },
                    {
                        "name": "dob",
                        "type": "date",
                        "options": []
                    },
                    {
                        "name": "nation",
                        "type": "text",
                        "options": []
                    },
                    {
                        "name": "weight",
                        "type": "number",
                        "options": []
                    },
                    {
                        "name": "weight_unit",
                        "type": "select",
                        "options": [
                            "kg",
                            "pound"
                        ]
                    }
                ],
                "finedPolicy": [
                    {
                        "sku_id": 553,
                        "fined_policy": [
                            {
                                "near_day": 1,
                                "far_day": 1,
                                "fined_mode": 1,
                                "value": 1,
                                "currency": ""
                            }
                        ]
                    },
                    {
                        "sku_id": 554,
                        "fined_policy": [
                            {
                                "near_day": 1,
                                "far_day": 3,
                                "fined_mode": 3,
                                "value": 11,
                                "currency": "€"
                            },
                            {
                                "near_day": 1,
                                "far_day": 3,
                                "fined_mode": 1,
                                "value": 12,
                                "currency": "€"
                            },
                            {
                                "near_day": 4,
                                "far_day": 5,
                                "fined_mode": 2,
                                "value": 99,
                                "currency": "€"
                            }
                        ]
                    }
                ]
            }
        }
    }
    
    
    
    Table 1.
    
    | product_sub_type | product_type | type_name      |
    |---------------   |:-----------: |----------------|
    |  7               |      1       | 一日游          |
    |  8               |      1       | 接驳            |
    |  9               |      1       | 酒店            |
    | 10               |      1       | WIFI           |
    | 11               |      2       | 票务            |
    | 12               |      3       | 跟团游          |
    | 13               |      4       | 机票            |
    | 14               |      5       | 签证            |
    | 15               |      6       | 邮轮            |
    
    Table 2.
    | product_region 	| product_sub_region			| name               |
    |----				|:------:						|--------------------|
    |  1 				|     						    | 美国               |
    |  2 				|    							| 加拿大             |
    |  3 				|    							| 拉美               |
    |  4 				|    							| 欧洲               |
    |  5 				|    							| 澳新               |
    |  7 				|    							| 非洲               |
    |  8 				|    							| 亚洲               |
    |  9 				|    							| 海岛目的地         |
    | 10 				|    							| 其他               |
    | 11 				|      1 						| 美西               |
    | 12 				|      1 						| 美东               |
    | 13 				|      1 						| 美中西             |
    | 14 				|      1 						| 佛州               |
    | 15 				|      1 						| 夏威夷             |
    | 16 				|      1 						| 阿拉斯加           |
    | 17 				|      1 						| 美南               |
    | 18 				|      2 						| 加东               |
    | 19 				|      2 						| 加西               |
    | 20 				|      3 						| 墨西哥             |
    | 21 				|      3 						| 其他拉美地区       |
    | 23 				|      5 						| 澳大利亚           |
    | 24 				|      5 						| 新西兰             |
    | 37 				|      7 						| 非洲               |
    | 38 				|      8 						| 亚洲其它           |
    | 39 				|      8 						| 中国               |
    | 40 				|      9 						| 海岛               |
    | 41 				|      9 						| 大洋洲             |
    | 42 				|     10 						| 其他               |
    | 43 				|      4 						| 北欧               |
    | 44 				|      4 						| 中欧               |
    | 45 				|      4 						| 东欧               |
    | 46 				|      4 						| 西欧               |
    | 47 				|      4 						| 南欧               |
    | 48 				|      4 						| 英国               |
    | 49 				|      4 						| 俄罗斯             |
    | 50 				|      3 						| 古巴               |
    | 51 				|      4 						| 爱尔兰             |



