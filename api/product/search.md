# 产品详情

### 描述

根据产品ID获取产品详情信息。数据结构根据你产品所属产品线，结构有所不同，在做业务处理时，请遵守产品线数据类型处理。

数据类型请参考 [这里](../../datastruct/product.md)

### API地址

    /v1/product/search

### 描述

| 参数            | 类型          | 是否必须 | 描述             |
| -------------- |:------------:| --------:| :-----------------|
| product_line   | string       |  否      | 搜索产品线  activity, tour |
| region         | string       |  否      | 区域信息   美国, 美东, 美西 等 |

### 描述

```javascript
{
    "product_line": "tour",
    "region" : "美国"
}
```

### 返回示例

```javascript
{
    "code": 0,
    "msg": "succ",
    "data": [
        {
            //产品线
            "product_line" : "activity",
            //产品名称
            "name" : "【穿越之旅】雷尼尔火山一日游·雷尼尔....",
            //产品ID
            "product_id" : 58839,
            //建议零售价 美元
            "advertised_price": "50.0000",
            //简要描述
            "brief_description" : "★ 用最短的时间穿越北美第一火山！(最短的时间，穿越北美第一火山)<br> ★ 畅游：克莉丝汀瀑布、那拉达瀑布、冰川远眺、天堂游客中心、倒影湖、玛莎瀑布、天堂草甸子等多处景点！",
            
            //***** 以下数据结构 activity tour 产品线适用
            
            //行程花费时间
            "duration" : 1,
            //行程花费时间单位 day,hour,minute
            "duration_type" : "day",
            //图片地址
            "image_url":"http://dn-toursforfun.qbox.me/images/201608081470682502_57a8d5863dd9c_watermark_800_800.jpg",
            //出发城市
            "departure_city_name": [
                {
                    "departure_city_name": "旧金山"
                },
                {
                    "departure_city_name": "圣何塞"
                },
                {
                    "departure_city_name": "旧金山湾区"
                }
            ],

            //结束城市（可多个）
            "return_city_name": [
                {
                    "return_city_name": "旧金山"
                },
                {
                    "return_city_name": "圣何塞"
                },
                {
                    "return_city_name": "旧金山湾区"
                }
            ],

            //最后更新时间
            "updated_at":1483018903, 

            //所属区域
            "region_chinese_name":"美国",
            "region":"us",
            "sub_region_chinese_name":"美东",
            "sub_region":"east"
        }
    ]
}
```



