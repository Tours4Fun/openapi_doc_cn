# 产品列表

### 描述

根据`地区`、`产品线` 等获取产品列表


### API地址

    /v2/product/list

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| region     | string  |  否   | 地区  |
| product_line     | string  |  否   | ttd or tour  |
| page   | int  |  否   | 默认1  |
| page_size   | int  |  否   | 每页条数,默认20  |
| keyword   | string  |  否   | 关键字,例如产品名称  |

注意：`region`,`product_line`,`keyword`三个参数至少有一个

region数据源:
美国,加拿大,拉美,欧洲,澳新,邮轮目的地,非洲,亚洲,海岛目的地,其他,美西,美东,美中西,佛州,夏威夷,阿拉斯加,美南,加东,加西,墨西哥,其他拉美地区,欧洲,澳大利亚,新西兰,加勒比航线,墨西哥航线,阿拉斯加航线,夏威夷航线,百慕大航线,地中海航线,北欧航线,加拿大-新英格兰航线,亚洲航线,极地航线,环球航线,澳大利亚-新西兰航线,非洲,亚洲其它,中国,海岛,大洋洲,其他,北欧,中欧,东欧,西欧,南欧,英国,俄罗斯,古巴,爱尔兰

### 参数实例

    {
    	"product_line" : "tour"
    }


### 返回示例

	{
        "code": 0,
        "msg": "success",
        "data": {
            //列表总数
            "count": "8851",
            //当前页数
            "page": "1",
            //每页记录数
            "page_size": "20",
            "products": [
                {
                    //产品id
                    "product_id": "13374",
                    //产品老id
                    "product_id_old": "103",
                    //产品名称
                    "name": "洛杉矶迪斯尼乐园超值欢乐一日游",
                    //产品图片
                    "image_url": "http://dn-toursforfun.qbox.me/images/201504271430120624_553de8b074648_watermark_800_800.jpg",
                    //产品线
                    "product_line": "activity",
                    //产品时长
                    "duration": "1.0",
                    //产品时长单位
                    "duration_type": "day",
                    //产品子区域
                    "sub_region": "west",
                    //产品子区域中文名称
                    "sub_region_chinese_name": "美西",
                    //产品区域
                    "region": "us",
                    //产品区域中文名称
                    "region_chinese_name": "美国",
                    //建议价格
                    "advertised_price": "20.700001",
                    //出发城市
                    "departure_city": [
                        {
                            "id": 1,
                            "name_en": "Los Angeles",
                            "name": "洛杉矶"
                        }
                    ],
                    //结束城市
                    "return_city": [
                        {
                            "id": 1,
                            "name_en": "Los Angeles",
                            "name": "洛杉矶"
                        }
                    ],
                    //途径城市
                    "visited_city": [
                        {
                            "id": 1,
                            "name_en": "Los Angeles",
                            "name": "洛杉矶"
                        }
                    ]
                },
                {
                    "product_id": "13527",
                    "product_id_old": "240",
                    "name": "一日夏威夷大岛风情游/Big Island One Day Tour",
                    "image_url": "http://dn-toursforfun.qbox.me/images/bida.jpg",
                    "product_line": "activity",
                    "duration": "11.5",
                    "duration_type": "hour",
                    "sub_region": "hawaii",
                    "sub_region_chinese_name": "夏威夷",
                    "region": "us",
                    "region_chinese_name": "美国",
                    "advertised_price": "310.000000",
                    "departure_city": [
                        {
                            "id": 162,
                            "name_en": "Honolulu",
                            "name": "檀香山"
                        }
                    ],
                    "return_city": [
                        {
                            "id": 162,
                            "name_en": "Honolulu",
                            "name": "檀香山"
                        }
                    ],
                    "visited_city": [
                        {
                            "id": 162,
                            "name_en": "Honolulu",
                            "name": "檀香山"
                        }
                    ]
                }
            ]
        }
    }


