# 产品信息

### 描述

根据产品编号，批量获取途风产品信息


### API地址

    /ctrip/product/detail

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| ctrip_product_ids     | string  |  是   | 产品编号  |

### 参数示例

```javascript
{
	"ctrip_product_ids":["4512-101580837"]
}
```

### 返回示例

```javascript
{
    "code": 0,
    "msg": "success",
    "data": {
        "4512-101580837": {
            "base": {
                "info": {
                    "status": 1,
                    "category_name": "一日游",
                    "category_id": 38,
                    "product_name": "【品味佳酿】坦莫宁山酒庄半日游 (布里斯班出发)",
                    "sub_name": null,
                    "duration": 4,
                    "duration_type": "hour",
                    "provider_product_name": "【品味佳酿】坦莫宁山酒庄半日游 (布里斯班出发)",
                    "product_code": "4512-101580837",
                    "currency": "USD",
                    "departure_city": [
                        {
                            "city_id": 236
                        }
                    ],
                    "return_city": [
                        {
                            "city_id": 248
                        }
                    ],
                    "property_list": [
                        "无购物"
                    ]
                },
                "image": [
                    "http://dn-tffimg.qbox.me/7c/d0/6c3/441/4dd8548c19a3ce437e06da.png?imageView2/1/q/85/format/jpg",
                    "http://dn-tffimg.qbox.me/11/90/b1b/22c/80ec26e7c9f436f7ba3dcc.png?imageView2/1/q/85/format/jpg",
                    "http://dn-tffimg.qbox.me/16/fc/7e7/370/3ce6d9a3af3320d8c3b451.png?imageView2/1/q/85/format/jpg",
                    "http://dn-tffimg.qbox.me/35/29/a5c/978/9932fc0f9fef7348fe80ed.png?imageView2/1/q/85/format/jpg",
                    "http://dn-tffimg.qbox.me/4f/58/047/23f/5432d818122bdd2f404c1d.png?imageView2/1/q/85/format/jpg",
                    "http://dn-tffimg.qbox.me/b7/f1/937/7a4/62e8b4e37c2f7212fe65e1.png?imageView2/1/q/85/format/jpg"
                ],
                "work_time": {
                    "name": "途风工作时间",
                    "time_zone": "(UTC+08:00)北京时间",
                    "begin_time": "9:00",
                    "end_time": "18:00",
                    "work_days": [
                        "周一",
                        "周二",
                        "周三",
                        "周四",
                        "周五"
                    ],
                    "work_on_vacation": "0"
                },
                "book_info": {
                    "booking_contact": "Jeff&Lucy",
                    "order_notify_method": [
                        "手机",
                        "邮件"
                    ],
                    "booking_phone": "18190759662",
                    "booking_email": "service@toursforfun.cn",
                    "booking_emergency_contact": "预订部",
                    "booking_emergency_phone": "18190759662",
                    "order_confirm_method": "供应商人工确认",
                    "exchange_mode": "携程确认单",
                    "need_delivery": "0",
                    "verify_days": "0",
                    "is_verify_on_weekend": "0",
                    "is_verify_on_holiday": "0"
                }
            },
            "description": {
                "itinerary_introduction": null,
                "product_introduction": "<b>【行程路线】</b>\r\nHeritage Estate酒庄>>雪松溪酒庄(Cedar Creek Estate Winery) >>坦莫宁山酿酒厂(Tamborine Mountain Distillery) >>德国小镇(Gallery Walk) \r\n\r\n<b>【行程介绍】</b>\r\n如果您想在号称黄金海岸的后花园品尝最地道的酿酒，那您绝对不能错过这趟坦伯林山酒庄半日游，昆士兰州里有许多屡获殊荣的酒庄，这趟旅程带您深入了解超过25年历史的雪松溪酒庄以及Heritage Estate酒庄，品尝不同款式的当地葡萄酒，在此享用下午茶。若您好奇酿酒的过程，那您在参访坦莫宁山的酿酒厂时，绝对能得到最专业的解答，还能一品酿酒厂中的白酒及烈酒。这趟旅程也将带您探索昆士兰州最好的艺术及手工艺中心—德国小镇(自由时间)。在往返的途中，请尽情享受窗外如画的风景，当巴士穿越壮观的Scenic Rim Country时，请别吝啬拿出您的相机，拍下这个曾经是具大火山群的地点，将风景纪录于您微醺的回忆里。\r\n\r\n<b>【出发地点及时间】</b>\r\n* 活动时长：约4.5小时(中午12:30pm出发，约下午5:00pm后回程)\r\n* 集合地点：Bus Stop 125, 161 Roma Street, Brisbane City, Queensland Australia\r\n- 巴士站即在布里斯班转运中心外头，对面是警察大楼的正门口\r\n- 请提早10分钟到指定集合地点，携带您的换票证Voucher办理报到",
                "hight_light": {
                    "light_1": "★ 在号称黄金海岸的后花园品尝最地道的酿酒及不同款式的当地葡萄酒",
                    "light_2": "\r\n★ 带您探索昆士兰州最好的艺术及手工艺中心—德国小镇，含自由活动时间",
                    "light_3": ""
                },
                "attractions": [
                    {
                        "ctrip_attraction_id": 9996,
                        "attraction_name": "拉罗什吉永",
                        "country_name": "法国"
                    }
                ]
            },
            "book_notice": {
                "tour_package_include": "不包含司机与导游服务小费(自由给予)\r\n不包含旅游保险(强烈建议您购买)\r\n不包含行程中的市区指定酒店接送加价费\r\n不包含所有个人费用和饮食，行程中的自费项目(价格会因为季节变化而有所调整，最终请以当地景点门市价格为标准)",
                "tour_package_exclude": "不包含司机与导游服务小费(自由给予)\r\n不包含旅游保险(强烈建议您购买)\r\n不包含行程中的市区指定酒店接送加价费\r\n不包含所有个人费用和饮食，行程中的自费项目(价格会因为季节变化而有所调整，最终请以当地景点门市价格为标准)",
                "notice": "* 该团我们以澳元做为团费结算货币，因为澳元和美元之间每日汇率都有所不同，所以您不同时间预订的行程价格与网页上面固定显示的价格会有所差别，最终价格请以途风当日系统核算后的价格作为您的最终购买价格。\r\n* 请于订购成功后，将收到的Voucher(非确认信)自行打印出来，于参加行程时提供给现场人员收票使用。Voucher视同正式票券，不可擅自毁损或涂改，亦不可转让他人使用。如您未如期收到Voucher，请务必再次确认，若因您的疏忽而无法将Voucher印出而导致行程无法进行，我们将视为是您自己造成的疏失，不允许退费。\r\n* 许多景点可能因公众假期或特殊事项停止或调整营业时间，若是因为顾客个人未加确认而造成本身行程的权益受损，将不得以此要求赔偿。\r\n* 未满18岁之未成年人，需由家长陪同成行，参加行程请携带护照以备查验。请确认您的护照及签证有效期限为6个月以上。\r\n* 若因为个人因素没有准时抵达出发地点，造成行程延误或取消，我们将视为是您自己造成的疏失，并无法要求退费。\r\n* 所有行程或节目安排皆按当地状况决定，如果因为天气、酒店或航班等无法预测之因素调整，不得以此要求补偿。\r\n* 请衡量您的健康状况参加适合的行程，若因个人身体状况问题无法完成行程，不得以此要求补偿。\r\n* 建议穿着半正式休闲套装；请自备保暖衣物；建议携带相机、遮阳帽、太阳眼镜及饮用水。\r\n* 因行程中含品酒活动，参加者须年满18岁及以上；此行程不适合轮椅使用者。\r\n* 若因路况或天气状况不佳，为了旅客的舒适，司机导游保有更换行程顺序或缩短行程的权力。\r\n* 此行程4人以上即可出团，低于4人预订请联系客服咨询所选出发日是否可以出团。\r\n* 请提早10分钟到指定集合地点，携带您的换票证Voucher办理报到。\r\n* 此行程报价及出团日期仅供参考，请与客服二次确认为准！\r\n* 巴士上禁止饮食、携带行李箱或婴儿车上车。\r\n* 因有品酒行程，预订者须年满18岁即可预订。\r\n\r\n【取消条款】\r\n本产品一经售出，不可退票及改签，敬请谅解。圣诞节期间可能会有预订不成功的风险，客服同事将为您做二次确认，请以确认后结果为准，敬请谅解。",
                "product_instruction": {
                    "instruction_1": "成人：18岁及以上\r\n未满18岁不能预订该产品。",
                    "instruction_2": "12:30:00+布里斯班(Brisbane)+Bus Stop 125, 161 Roma Street, Brisbane City, Queensland Australia+",
                    "instruction_3": null
                }
            },
            "ext_info": [
                {
                    "ext_name": "出发酒店地址（英文）",
                    "ext_type": "text",
                    "ext_options": []
                }
            ],
            "customer_maintain_info": {
                "contact_info": [
                    "联系手机",
                    "联系邮箱地址"
                ],
                "customer_info_type": "3",
                "customer_info_template": "-1",
                "customer_info_items": [
                    {
                        "name": "中文姓名",
                        "check": 1
                    },
                    {
                        "name": "英文姓名",
                        "check": 1
                    },
                    {
                        "name": "护照",
                        "check": 1
                    },
                    {
                        "name": "性别",
                        "check": 1
                    },
                    {
                        "name": "体重（kg）",
                        "check": 1
                    }
                ]
            },
            "options": [
                {
                    "info": {
                        "name": null,
                        "elements_name": "\"\\u6210\\u4eba-\\u4e0d\\u5347\\u7ea7(\\u81ea\\u884c\\u524d\\u5f80)\"",
                        "status": 1,
                        "advance_booking_days": 4,
                        "advance_booking_time": "17:05",
                        "min_book_num": 1,
                        "max_book_num": 99,
                        "option_code": "1_1328369619-113655",
                        "language": [
                            "英文"
                        ]
                    },
                    "price": [
                        {
                            "date": "2018-04-29",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 86,
                            "retail_price": 73
                        }
                    ]
                },
                {
                    "info": {
                        "name": null,
                        "elements_name": "\"\\u6210\\u4eba-\\u5347\\u7ea7(\\u9152\\u5e97\\u81f3\\u7231\\u5c14\\u5229\\u6e2f\\u5df4\\u58eb\\u5f80\\u8fd4)\"",
                        "status": 1,
                        "advance_booking_days": 4,
                        "advance_booking_time": "17:05",
                        "min_book_num": 1,
                        "max_book_num": 99,
                        "option_code": "1_1328369619-113658",
                        "language": [
                            "英文"
                        ]
                    },
                    "price": [
                        {
                            "date": "2018-04-29",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-29",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-01",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-02",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-03",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-04",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-05",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-06",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-07",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-08",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-09",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-10",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-11",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-12",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-13",
                            "settlement_price": 170,
                            "retail_price": 198
                        }
                    ]
                },
                {
                    "info": {
                        "name": null,
                        "elements_name": "\"\\u5c0f\\u5b69-\\u4e0d\\u5347\\u7ea7(\\u81ea\\u884c\\u524d\\u5f80)\"",
                        "status": 1,
                        "advance_booking_days": 4,
                        "advance_booking_time": "17:05",
                        "min_book_num": 1,
                        "max_book_num": 99,
                        "option_code": "2_1328369619-113655",
                        "language": [
                            "英文"
                        ]
                    },
                    "price": [
                        {
                            "date": "2018-04-29",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-29",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-01",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-02",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-03",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-04",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-05",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-06",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-07",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-08",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-09",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-10",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-11",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-12",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-13",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-04-29",
                            "settlement_price": 0,
                            "retail_price": 0
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 0,
                            "retail_price": 0
                        }
                    ]
                },
                {
                    "info": {
                        "name": null,
                        "elements_name": "\"\\u5c0f\\u5b69-\\u5347\\u7ea7(\\u9152\\u5e97\\u81f3\\u7231\\u5c14\\u5229\\u6e2f\\u5df4\\u58eb\\u5f80\\u8fd4)\"",
                        "status": 1,
                        "advance_booking_days": 4,
                        "advance_booking_time": "17:05",
                        "min_book_num": 1,
                        "max_book_num": 99,
                        "option_code": "2_1328369619-113658",
                        "language": [
                            "英文"
                        ]
                    },
                    "price": [
                        {
                            "date": "2018-04-29",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 86,
                            "retail_price": 73
                        },
                        {
                            "date": "2018-04-29",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-01",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-02",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-03",
                            "settlement_price": 96,
                            "retail_price": 82
                        },
                        {
                            "date": "2018-05-04",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-05",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-06",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-07",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-08",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-09",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-10",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-11",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-12",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-05-13",
                            "settlement_price": 170,
                            "retail_price": 198
                        },
                        {
                            "date": "2018-04-29",
                            "settlement_price": 0,
                            "retail_price": 0
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 0,
                            "retail_price": 0
                        },
                        {
                            "date": "2018-04-29",
                            "settlement_price": 10,
                            "retail_price": 9
                        },
                        {
                            "date": "2018-04-30",
                            "settlement_price": 10,
                            "retail_price": 9
                        },
                        {
                            "date": "2018-05-01",
                            "settlement_price": 10,
                            "retail_price": 9
                        },
                        {
                            "date": "2018-05-02",
                            "settlement_price": 10,
                            "retail_price": 9
                        },
                        {
                            "date": "2018-05-03",
                            "settlement_price": 10,
                            "retail_price": 9
                        },
                        {
                            "date": "2018-05-04",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-05",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-06",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-07",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-08",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-09",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-10",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-11",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-12",
                            "settlement_price": 18,
                            "retail_price": 21
                        },
                        {
                            "date": "2018-05-13",
                            "settlement_price": 18,
                            "retail_price": 21
                        }
                    ]
                }
            ]
        }
    }
}
```
