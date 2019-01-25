# Product Detail Info

### Description

    Get the product Detail Info

### API address

    ttd/product/detail

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| product_ids          | array         |     Yes     |   Product Ids[max:50]           |
| return_fields        | array         |     No      |   Optional Module:basic, info, departure, skuInfo, passengerForm, FinedPolicy[default:all modules]          |

```
basic : Product basic information, type, region, media, etc.
info : Product description information, group fee content, itinerary, etc.
departure : Product departure start/end time and location.
skuInfo : Product sku info and sale restriction.
passengerForm : Information that travellers need to fill out.
FinedPolicy : Cancel modification of penalty rules.
```

### Request parameter demo

	{
    	"product_ids":[102851680],
    	"return_fields":["basic", "info", "departure", "skuInfo","passengerForm","finedPolicy"]
    }

### Return field description

    basic[Product basic properties]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| product_id                        |     Product unique id                             |
| product_type                      |     Product type [See Table 1 For Details.]       |
| name                              |     Product name                                  |
| departure_city                    |     Departure city                                |
| -id                               |     City id                                       |
| -name_en                          |     English name                                  |
| -name                             |     Chinese name                                  |
| return_city                       |     Return city                                   |
| -id                               |     City id                                       |
| -name_en                          |     English name                                  |
| -name                             |     Chinese name                                  |
| activity_type                     |     Type of activity                              |
| duration                          |     Product duration                              |
| duration_type                     |     Product duration unit[min,hour,day]           |
| is_vega_show                      |     Show ticket[0=>No, 1=>Yes]                    |
| product_region                    |     Product region name                           |
| product_sub_region                |     Sub region name                               |
| language                          |     Service language                              |
| image_url                         |     Product image Url                             |
| video_url                         |     Product video Url                             |



    info[Product description]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| highlights                        |     Product highlights                            |
| summary                           |     Trip description       |
| notice                            |     Notice                                  |
| includes                          |     Cost includes                                |
| excludes                          |     Cost does not include                                            |
| package_special_note              |     Participation note                                  |
| price_special_note                |     Price note                                  |
| tips                              |     Tips                                   |
| how_to_use                        |     E-ticket usage                                  |
| airport_transfer_info             |     Transfer information                                  |
| contain_airport_transfer          |     0: not contain pick up and drop off; 1: contain pick up and drop off; 2: contain pick up; 3: contain drop off                              |
| is_welcome_board                  |     Pick-up card[1=>Yes, 0=>No]                              |
| flight_time_limit                 |     Flight information time limit unit[day]           |
| attractions                       |     Visited attractions                   |
| -city_id                          |     City id                    |
| -name                             |     Attractions name                    |
| -description                      |     Attraction description                    |
| cities                            |     Visited city                    |
| -city_id                          |     City id                    |
| -name                             |     City name                    |
| -description                      |     City description                    |
| ownexpenses                       |     Optional item                    |
| -ownexpense_id                    |     Item id                    |
| -name                             |     Item name                    |
| -description                      |     Item description                    |
| -price                            |     Item price description                    |
| -duration                         |     Item duration[day]                    |
| -tips                             |     Item tips                    |

    departure[Departure/end time and place]

| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| start_locations/end_locations     |     Departure/end time and location                            |
| location_status                   |     [1=>Fixed location+user to select;2=>Fixed location+only show;3=>user fillin]       |
| locations                         |          --                             |
| -departure_id                     |     Departure id                                |
| -start_time                       |     Start time                                |
| -end_time                         |     End time                                |
| -region                           |     Area                               |
| -location                         |     Location                                |
| -address                          |     Address                                |
| -tips                             |     Tips                                |
| -longitude                        |     Longitude                                |
| -latitude                         |     Latitude                                |
| -operations                       |     Available time[If it is empty, there is no date limit.]                                |
| --start_date                      |     Start date                                |
| --end_date                        |     End date                                |
| --sunday                          |     [1=>sunday usable,0=>not]                                |
| --monday                          |     [1=>monday usable,0=>not]                                 |
| --tuesday                         |     [1=>tuesday usable,0=>not]                                |
| --wednesday                       |     [1=>wednesday usable,0=>not]                                |
| --thursday                        |     [1=>thursday usable,0=>not]                                |
| --friday                          |     [1=>friday usable,0=>not]                                |
| --saturday                        |     [1=>saturday usable,0=>not]                                |


    skuInfo[Product optional sku info]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| sku_id                            |     Sku unique Id                           |
| display_name                      |     Display name                               |
| sku_name                          |     Sku name, Splicing according to attributes                               |
| min_age                           |     Minimum age limit[0=>not limit]                               |
| max_age                           |     Maximum age limit[0=>not limit]                               |
| min_guest_number                  |     Minimum purchase quantity                               |
| max_guest_number                  |     Maximum purchase quantity                               |
| sold_with_other_sku               |     Can not be booked separately, need to be sold with other sku                               |


    passengerForm[Traveler is scheduled to fill in the information]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| name                              |     Display name                           |
| type                              |     Form input type                               |
| options                           |     Input options                                 |

    finedPolicy[Cancel modification of penalty rules]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| sku_id                            |     Sku id                           |
| fined_policy                      |     Cancel modification of penalty rules                               |
| -near_day                         |     Number of days to start the rule                               |
| -far_day                          |     Rule end days                               |
| -fined_mode                       |     [1=>% of total group fee;2=>A fixed fee is charged per person;3=>A fixed handling fee per order]                               |
| -value                            |     Fee ratio or amount                               |
| -currency                         |     Amount of currency                               |




### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "102851680": {
                "basic": {
                    "product_id": 102851680,
                    "product_type": 11,
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
                    "activity_type": "景点门票",
                    "duration": 3,
                    "duration_type": "hour",
                    "is_vega_show": 0,
                    "product_region": "美国",
                    "product_sub_region": "美西",
                    "language": [
                        "English Audio",
                        "English Live"
                    ],
                    "image_url": [
                        "http://img1.dev5.tff.com/f1/windtour/0f/9d/tiyan3.jpg",
                        "http://img1.dev5.tff.com/f1/windtour/37/46/qa-title.png"
                    ],
                    "video_url": ""
                },
                "info": {
                    "highlights": "*途风和美国洛杉矶出团数量最大的巴士地接公司强强合作！*由洛杉矶最具经验的专职双语导游带您游览环球影城以及好莱坞，您将在这里领略到著名影视城的独特魅力。",
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
                "skuInfo": [
                     {
                         "sku_id": 553,
                         "display_name": "2b",
                         "sku_name": "时间:19:00|时长:120 hours|test other|成人",
                         "min_age": 0,
                         "max_age": 0,
                         "min_days_before_departure": 0,
                         "min_guest_number": 1,
                         "max_guest_number": 3,
                         "sold_with_other_sku": "557,558,559"
                     },
                     {
                         "sku_id": 554,
                         "display_name": "",
                         "sku_name": "时间:15:00|时长:120 hours|test other|成人",
                         "min_age": 0,
                         "max_age": 0,
                         "min_days_before_departure": 0,
                         "min_guest_number": 1,
                         "max_guest_number": 3,
                         "sold_with_other_sku": ""
                     }
                ],
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

| product_type     | product_type_name      |
|---------------   |:-----------------------|
|  7               |      TTD-一日游         |
|  8               |      TTD-接驳          |
|  9               |      TTD-酒店          |
| 10               |      TTD-WIFI         |
| 11               |      票务             |
| 12               |      跟团游           |
| 13               |      机票             |
| 14               |      签证              |
| 15               |      邮轮              |



