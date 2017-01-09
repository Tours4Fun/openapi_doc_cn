# 产品详情

### 描述

根据产品ID获取产品详情信息。数据结构根据你产品所属产品线，结构有所不同，在做业务处理时，请遵守产品线数据类型处理。

数据类型请参考 [这里](../../datastruct/product.md)

### API地址

    /v1/product/detail

### 描述

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  是   | 产品ID好  |

### 描述

```javascript
{
    "product_id": 101561985
}
```

### 返回示例

```javascript
{
    "code": 0,
    "msg": "succ",
    "data": {
        "base":{
            "updated_at":1483018903, //最后更新时间
            //产品名称
            "name":"【穿越之旅】雷尼尔火山一日游·雷尼尔国家公园+克莉丝汀瀑布+那拉达瀑布+冰川远眺+天堂游客中心+倒影湖+玛莎瀑布+天堂草甸子",
            "advertised_price":"50.0000", //建议价格
            "departure_city":"西雅图", //出发城市
            "return_city":"西雅图", //返回城市
            "duration":"1.0", //行程时间
            "duration_type":"day", //行程时间单位 day,hour,minute
            "max_child_age":0, //最大小孩年龄
            "min_days_before_departure":0, //提前预定天数
            "hotel_pickup":0, //是否支持酒店接送
            "is_departure_time":0,
            "is_shopping_tour":0, //是否是购物团
            "min_guest_number":1, //最小出团人数
            "type_id":10101, //TODO what is this?
            "show_ownexpense":1, //是否应该显示自费项目
            "product_id":58839, //产品ID
            //图片地址
            "image_url":"http://dn-toursforfun.qbox.me/images/201608081470682502_57a8d5863dd9c_watermark_800_800.jpg",
            "is_pickup":0, //有无出发接送服务
            "is_dropoff":0, //有无到达接送服务
            "subcode_note":"如果客人有8岁以下儿童参团，请特别告知供应商，以便供应商提前安排儿童安全座椅(导游团上收取儿童安全座椅费用$8/天)",
            "is_backend":1,  //TODO what is this?
            "type_descr":"国家公园",
            //开始城市
            "departure_city_name":[
                {
                    "departure_city_id":595,
                    "language_id":3,
                    "departure_city_name":"西雅图"
                }
            ],
            //结束城市
            "return_city_name":[
                {
                    "return_city_id":595,
                    "language_id":3,
                    "return_city_name":"西雅图"
                }
            ],
            "product_line":"activity",//产品线
            "region_chinese_name":"美国",
            "region":"us",
            "sub_region_chinese_name":"美东",
            "sub_region":"east"
        },
        "info":{
            //简要描述
            "brief_description":"★ 用最短的时间穿越北美第一火山！(最短的时间，穿越北美第一火山)<br> ★ 畅游：克莉丝汀瀑布、那拉达瀑布、冰川远眺、天堂游客中心、倒影湖、玛莎瀑布、天堂草甸子等多处景点！",
            //消息描述
            "full_description":"",
            //摘要
            "summary":"就像纽约有自由女神像、旧金山有金门大桥，华盛顿州有雷尼尔火山....",
            //团费说明
            "price_special_note":"<div class="pr_2"> <div class="p_p"><div class="p_p">*成人：12岁及以上</div> <div class="p_p">*小孩： 12岁以下 </div> </div>",
            //电子票说明 电子票使用
            "eticket_special_note":"***【参团须知】*** * 为确保您的行程顺利，....",
            //提示
            "tips":"",
            //产品提示
            "product_tips":"如果客人有8岁以下儿童参团，请特别告知供应商，以便供应商提前安排儿童安全座椅(导游团上收取儿童安全座椅费用$8/天)"
        },
        "language":[

        ],
        //途径景点
        "attraction":[
            {
                "attraction_id":26859,
                //排序
                "index":0,
                //花费时间
                "duration":"0.0",
                //花费时间单位
                "duration_type":"hour",
                "is_optional":0,
                //名称
                "name":"雷尼尔山国家公园",
                //描述
                "description":"瑞尼尔山国家公园(Mount Rainier National Park)也译作雷尼尔山国家公园，是一座位于美国华盛顿州皮尔斯郡东南的国家公园。建园于1899年3月2日，是美国第五座国家公园。公园面积为368平方英里(954平方公里)，包括了瑞尼尔山全境——一座14,410呎(4,392米)高的层状火山。这座山从周遭的平地中陡然升起，使得园区海拔分布从1600呎(490米)到超过14,000呎(4,300米)。"
            }
        ],
        //途径城市
        "city":[
            {
                "city_id":595,
                "index":0,//排序
                //城市名称
                "name":"西雅图",
                //城市描述
                "description":""
            }
        ]
    }
}
```



