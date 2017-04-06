# 产品详情

### 描述

根据产品ID获取产品详情信息。数据结构根据你产品所属产品线，结构有所不同，在做业务处理时，请遵守产品线数据类型处理。

数据类型请参考 [这里](../../datastruct/product.md)

### API地址

    /v1/product/detail

### 参数

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| :-----------------|
| product_id     | int  |  是   | 产品ID号  |

### 参数示例

```javascript
{
    "product_id": 101561985
}
```

### 返回示例

```javascript
{
  "code": 0,
  "msg": "success",
  "data": {
    "base": {
      "updated_at": 1485240198,
      "name": "<p>美东豪华之旅：纽约精华全览、古老波士顿、华盛顿游船赏景、尼亚加拉大瀑布、新鲜龙虾餐</p>\r\n",
      "image_url": "Lake-Ontario-ECAN8D(p).jpg",
      "advertised_price": "1000.0000",
      "stock_status":1,
      "duration": "6.00",
      "duration_type": "day",
      "max_child_age": 0,
      "min_days_before_departure": 0,
      "min_guest_number": 1,
      "display_itinerary_note": 1,
      "show_ownexpense": 1,
      "visa_passport": 1,
      "is_pickup": 2,
      "is_dropoff": 2,
      "product_id": 100009369,
      "product_line": "tour",
      "departure_city_name": [
        {
          "departure_city_id": 496,
          "departure_city_name": "Dali"
        },
        {
          "departure_city_id": 18,
          "departure_city_name": "Lago del la Ciudad de Havazu"
        },
        {
          "departure_city_id": 20544,
          "departure_city_name": "Niagara Falls"
        },
        {
          "departure_city_id": 20634,
          "departure_city_name": "Niagara Power Vista"
        }
      ],
      "return_city_name": [
        {
          "return_city_id": 619,
          "return_city_name": "Queenstown"
        },
        {
          "return_city_id": 23998,
          "return_city_name": "中国国内机场/市内"
        }
      ],
      "region_chinese_name": "亚洲",
      "region": "asia",
      "sub_region_chinese_name": "中国",
      "sub_region": ""
    },
    "info": {
      "brief_description": "<p>马杜加里岛(Madoogali)几乎完全包裹在郁郁葱葱的热带植被中，椰子树、榕树、无处不在的异国芳香，绿松石般的海洋亲吻着柔软的珊瑚白沙滩，这一切美景都等着您的品鉴.<br />\r\n一个独特又从未被触碰过的天堂，专为那些少数特别的人追寻最荣耀的大自然所提供。</p>\r\n",
      "full_description": "",
      "airport_transfer_info": "",
      "notice": "<strong>***2014途风大礼包***</strong><br>\r\n即日起，参加行程的贵宾可获赠每人$100.00的超级大礼包！！！<br>\r\n★ 2 餐美味中式海鲜自助午餐，价值$30.00!!<br>\r\n★ 马戏团大酒店内世界最大室内主题公园的2大热门娱乐项目，价值$25.00!!<br>\r\n★ 马戏团大酒店内世界最大永久马戏团的精彩表演，价值$10.00!!<br>\r\n★ 马戏团大酒店内的各式餐厅礼品店折扣券，价值$20.00 !!<br>\r\n★ 马戏团大赌场赠送赌金，价值$15.00 !!<br>\r\n（以上赠送项目详情请以团上导游确认的信息为准）<br>\r\n<font color=#f7860f>送餐温馨提示：</font><br>\r\n豪华自助午餐仅限于拉斯维加斯，用餐地址4300 E. Sunset Rd., C-1, Henderson, NV 89014。享用自助午餐的客人，需支付$1.00小费。<br><br>\r\n\r\n<strong>***预订须知***</strong><br>\r\n1).新年，劳工节，国庆日，感恩节，圣诞节或其他长周末假期期间，团费会有适当的调升，请在订团前与我们确认最终价格。<br>\r\n2).行程先后次序会因出发日期不同而作调整，最终行程请以我们的确认为准。<br>\r\n3).2014 年4月1日起，拉斯维加斯酒店可付费升级到拉斯维加斯大道上的Paris酒店，地段更好，品尝丰盛大餐，观看精彩表演。如需升级请联系我们取得报价。<br>\r\n4)黄石团行程是途风夏季销售最热门的行程路线之一， 很多行程在很短的时间内都会销售一空。<br>\r\n5)为了保证所有贵宾的旅行安排顺畅，我们强烈建议您提前一至二个月预定黄石团行程。<br>\r\n6)我们会在每个工作日下午六时（洛杉矶时间）更新我们的黄石团剩余座位情况。<br>\r\n7)请务必在预定行程并收到我们的确定涵以后再预定机票。我们会在您预订行程之后，1-2个工作日（美国时间）内通知您是否确定还有剩余座位；对于未收到我们的确认，却提前预定机票的贵宾，有可能会因为没有位置而耽误到您的旅行计划，届时途风概不负担责任，敬请谅解。<br>\r\n8)为了节省您的额外开支，请各位游客尽量将到达时间安排在我们免费的接应时间段。<br>\r\n9)如需以下额外服务，请发邮件或致电途风：<br>\r\n* 在免费接机时段以外到达；<br>\r\n* 航班临时改变或延迟，需要额外接应服务； （在我们工作时段内）<br>\r\n* 一个订单需要多次接应服务。<br>\r\n<br>\r\n<strong>***参团须知***</strong><br>\r\n凡参加行程会入住拉斯维加斯酒店的客人，须年满21岁或有21岁以上客人陪同。<br>\r\n在每年的4-5月期间，受年初大雪的影响，黄石公园内的部分景点还未开放；另外在10月期间，由于天气骤变等原因，正常游览顺序及内容可能会受一定影响。<br>\r\n我们可能会通过安排其他旅游景点或者增加在黄石公园停留时间等措施，尽量弥补给各位贵宾造成的不便，也请您谅解我们，并以导游在团上的最终安排为准，感谢您的理解及配合！<br>\r\n在旺季期间，由于酒店房间供应紧张，我们可能会为您更换同等级的酒店，谢谢您的理解及支持！<br><br>\r\n\r\n<font color=#f7860f><strong>变更或修改条款</strong></font><br>\r\n*由于黄石行程十分受欢迎，我们替您预留座位。如果您在确认订单后需要更改出团日期或减少参团人数，请务必提前17天通知，否则将按照以下条款收取一定的费用以及$30的修改订单费用。<br>\r\n1)出团前10-16天，我们将收取团费的30%作为罚款<br>\r\n2)出团前6-9天，我们将收取团费的50%作为罚款<br>\r\n3)出团前5天(工作日)以内，我们将收取全部团费作为罚款<br>\r\n\r\n<font color=#f7860f><strong>买二送一免费者取消条款</strong></font><br>\r\n*我们替享受优惠者预留座位，享受该优惠的订单中如要取消免费者，请务必提前10天通知，否则将按照以下条款收取一定的取消费用以及$30的修改订单费用。<br>\r\n1)出团前6-9天，我们将收取$50每人的罚款<br>\r\n2)出团前1-5天(工作日)，我们将收取$100每人的罚款<br>\r\n3)出团当天不出现，导游将在团上收取$150每人的罚款<br><br>",
      "includes": "<LI>空调巴士或者中巴接送，每个预订单提供指定机场的免费接送机服务(第一天洛杉矶机场的免费接机时间为: 美国国内航班8:30am-10:00pm;国际航班8:30am-9:30pm)。</LI>\r\n<LI>九晚酒店住宿, 所有酒店提供标准间, 双人床 </LI>\r\n<LI>精心安排旅馆酒店及大型巴士, 让您的旅程舒适又安全 </LI>\r\n<LI>当地最具经验的专职双语导游和超过10年驾驶经验的车长</LI>\r\n<LI>西峡谷门票(每人$80.00)(含一顿午餐：印第安烤肉或中式便当餐)</LI>",
      "excludes": "<li>不提供您往返出发地的机票和指定机场的相关交通费用</li>\r\n<li>所有个人费用和饮食，行程中的门票或自费项目(自费项目和价格可能会因为季节变化而有所调整，最终请以出团当天的实际项目和当地公园门市价格为准)。</li><br>\r\n-大峡谷国家公园门票：$10.00/人【南峡谷行程】<font color=#f7860f>这是您在团上必付的费用</font><br>\r\n-玻璃桥门票：$35.00/人【西峡谷行程】<br>\r\n-西峡谷直升机+游船：$205.00/人【西峡谷行程】<br>\r\n-拉斯维加斯360度夜景直升机：$139.00/人【西峡谷行程】</LI><br>\r\n-拉斯维加斯夜晚深度游：$25.00/人<br>\r\n-拉斯维加斯大型歌舞表演：$83.00/人起<br>\r\n-拉斯维加斯奇幻魔术表演：$98.00/人<br>\r\n-世界第一秀-水之梦：$160.00/人<br>\r\n-太阳剧团-奇异剧场：$119.00/人<br>\r\n-太阳马戏团-卡秀：$120.00/人<br>\r\n-最性感火辣的脱衣舞秀（18禁）：$65.00/人<br>\r\n-纳帕谷+熊世界+大盐湖+国家公园+燃油附加費：以上为组合套餐，费用为$45.00/人<span style=color:#f7860f>(这是您在团上必付的项目，导游会在行程第五天收取此费用)</span> <br /> \r\n- 羚羊彩穴吉普车：$37.00/人(08:00am)<br>\r\n- 旧金山海湾游船：$36/成人；$24.00/小孩</LI>\r\n<li>不包括接送机服务费：$3.00/人</li>\r\n<LI>不包括提供给导游和司机的服务费(每位客人支付司机及导游服务费：共$7.00/每天) </LI>",
      "package_special_note": "<br>\r\n<span style=\"font-weight:bold;\">【航班注意事项】：</span><br>\r\n<LI>请注意协调您的航班和旅行团行程的时间，避免误机。<br>\r\n我们建议您在收到行程确认邮件后再预订机票。您的预订通常会在1-2个工作日内得到确认。</li>\r\n<br>\r\n<span style=\"font-weight:bold;\">【预定注意事项】：</span><br>\r\n<li>我们替您预留座位，如果您在确认订单后需要更改出团日期，请务必提前17天通知，否则将按照<b>变更或修改条款</b>收取一定的费用以及<b style=\"font-weight:bold\">$30的修改订单费用</b>。\r\n<li>黄石团行程是途风夏季销售最热门的行程路线之一， 很多行程在很短的时间内都会销售一空。为了保证所有贵宾的旅行安排顺畅，我们强烈建议您提前一至二个月预定黄石团行程。<br>\r\n我们会在每个工作日下午六时（洛杉矶时间）更新我们的黄石团剩余座位情况。</li><br>\r\n\r\n<span style=\"font-weight:bold;\">【行程注意事项】：</span><br>\r\n  <LI>搭乘飞机时，请随时扣紧安全带，以免乱流影响安全。 </li>\r\n  <LI><FONT color=#F7860F>行程先后次序可能会因出发日期而作调整, 但是行程内容完全一样。</FONT></li>\r\n  <LI>住宿饭店时请随时将房门扣上安全锁，以策安全；勿在灯上晾衣物；勿在床上吸烟，听到警报器响，请由紧急出口迅速离开。 </li>\r\n  <LI>每个酒店房间只安排两张床;三人同房如需加床请自行向酒店服务台查询。 </li>\r\n  <LI>团体需一起活动，途中若要离队需征得导游同意以免发生意外。 </li>\r\n  <LI>夜间或自由活动时间若需自行外出，请告知导游或团友，并应特别注意安全。 </li>\r\n  <LI>行走雪地及陡峭之路请谨慎小心。 </li>\r\n  <LI>遵守导游所宣布的观光区、饭店、游乐设施等各种场所的注意事项。 </li>\r\n  <LI>药物：胃肠药、感冒药、晕车药、私人习惯性药物。(视个人身体情况自行准备) </li>\r\n  <LI>如遇特别情形, (天气,修路,罢工,封山,旅游车特殊状况) 为保障旅客权益, 本公司保留调整取消行程的最终解释权。 </li>\r\n  <LI>春夏两季：请您注意穿著轻便的衣物和舒适的鞋子。<BR>\r\n    秋冬两季：请您注意穿著厚实的衣物以保暖。</LI>\r\n<LI>途风温馨提示：<BR>为保障您的个人财产安全，我们建议您在旅行期间随身携带个人贵重物品，不要将贵重物品遗留在大巴/酒店/景点/餐馆等地点；<BR>在任何情况及任何地点下失窃，造成个人财产损失，途风、地接社及司机、领队导游等均不负任何责任，请您悉知。</LI>",
      "price_special_note": "<style type=\"text/css\">\r\n<!--\r\n.STYLE4 {font-weight: bold; font-family: \"Times New Roman\", Times, serif; color: #F7860F;}\r\n.STYLE5 {color: #F7860F}\r\n-->\r\n</style>\r\n<div class=\"pr_2\">\r\n<div class=\"p_p\">\r\n  <p class=\"STYLE4\"> 买 二 送 一</p>\r\n  <p align=\"left\" class=\"STYLE5\">如：三个人住一个三人间的总价格=2x双人间单价+$120.00(附加费)</p>\r\n  <p align=\"left\" class=\"STYLE5\">＊凡获得买二送一优惠的所有客人均只获一房。</p>\r\n <p align=\"left\" class=\"STYLE5\">注意：以上所列价格是经原价调整之后的\"买二送一\"的价格。</p>\r\n\r\n <p align=\"left\" class=\"STYLE5\">*凡享受买二送一优惠的行程，如要取消其中的一人享受优惠者，请务必提前10天通知修改，否则将根据<strong>取消和退款条例</strong>收取相应的预定费用。</p>\r\n \r\n<p align=\"left\" class=\"STYLE5\">*我们特别为享受优惠者提前预留座位，如果享受该优惠的订单中有人当天未参加该团，地接社将会以现金的方式收取相应的罚款。</p>\r\n\r\n<div class=\"p_p\">*单人间价格是指一人单独享有一个酒店标准间的价格。</div>\r\n<div class=\"p_p\">*双人/三人/四人间是指双人/三人/四人共同享用一个酒店标准间的价格。  </div>\r\n<div class=\"p_p\">*三人/四人间价格不包括在房间里另加床位的价格,另加床位要在登记时单独提出要求。 </div> <div class=\"p_p\">*请注意：由于酒店标准间空间及所加床位有限，请客人自行向酒店服务台咨询加床事宜，途风不能保证加床成功。</div>\r\n\r\n<div class=\"p_p\">*一个房间最多只能容纳包括成人和小孩或婴儿在内共四人。\r\n</div>\r\n</div></div>",
      "eticket_special_note": "紧急联络电话：1-323-261-8811\r\n\r\nComfort Suites Rosemead \r\nTEL: (626) 228-0528\r\n9488 Valley Blvd., Rosemead, CA 91770\r\n\r\nBest Western Rowland Heights \r\nTEL: (626) 810-1818\r\n18880 E. Gale Ave., Rowland Heights, CA 91748\r\n\r\nHoliday Inn La Mirada\r\nAddress: 14299 Firestone Blvd, La Mirada, CA 90638\r\nTel: 714-739-8500\r\n\r\nHoward Johnson Hotel\r\nAddress: 222 West Houston Avenue, Fullerton, CA 92832\r\nTel: (714) 992-1700\r\n\r\n请注意：在旺季期间，由于酒店房间供应紧张，我们可能会为您更换同等级的酒店，谢谢您的理解及支持！!##!请提前向导游告知您参加的是双峡行程，两个峡谷都前往，以便导游进行安排。!##!!##!紧急联系电话:1-323-261-8811\r\n\r\n今天早上5:00am，请您在Circus Circus Hotel酒店的二楼电梯旁资讯台(Las Vegas,Circus Circus Skyrise Tower 2nd Floor Information)跟导游汇合。\r\n\r\nCircus Circus Hotel , Las Vegas\r\nAddress: 2880 Las Vegas Blvd S, Las Vegas, NV, 89109 United States\r\nTel: (702) 734-0410!##!紧急联络电话：1-323-261-8811\r\n\r\n请注意：在旺季期间，由于酒店房间供应紧张，我们可能会为您更换同等级的酒店，谢谢您的理解及支持！!##!!##!!##!!##!!##!",
      "tips": "womenrefgv",
      "additional_promotion": "frere",
      "credential": "werqw",
      "change_notice": "frgerefg",
      "auto_confirm": "frgevre",
      "travel_notice": "fghnbgfbhftgh",
      "product_tips": ""
    },
    "language": [
      {
        "language_type": "live",
        "name": "加泰罗尼亚语 Live",
        "icon": "catalan_live.jpg",
        "sort_order": 0
      },
      {
        "language_type": "audio",
        "name": "中文 Audio",
        "icon": "chinese_audio.jpg",
        "sort_order": 0
      }
    ],
    "itinerary": [
      {
        "day_no": 1,
        "itinerary_no": 1,
        "mileage": "3.26",
        "tips": "为了给各位贵宾提供更高效贴心的服务，如果您下单并支付全额团费的日期距离您选择的出团时间在3天及以上，我们100%保证为您保留座位。",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 1,
        "has_attraction": 1,
        "summary": "早上继续畅游尼加拉大瀑布之旅，前往位于尼加拉河上的公羊岛，欣赏白天的大瀑布，更有机会看到挂在瀑布上的彩虹，之后到位于美国瀑布旁的电影院欣赏大瀑布IMAX电影*，在IMAX电影院内感受震撼的音响及超大银幕，作为游览尼加拉大瀑布的完美结局；之后前往下一城市波士顿，晚上到达位于麻省的波士顿，首先当然要先品尝当地最有名的波士顿龙虾*作为晚餐，大小适中的波士顿龙虾，爽口甜美，非吃不可！",
        "title": "纽约市博物馆-纽约唐人街",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "Newark",
                  "pinyin": "N",
                  "alias": "",
                  "description": ""
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "city",
            "order": 7,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "Newark",
                  "pinyin": "N",
                  "alias": "",
                  "description": ""
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "attraction",
            "order": 2,
            "attraction_item": [
              {
                "duration": "1.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "纽约市博物馆",
                  "pinyin": "N",
                  "alias": "",
                  "description": "",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 345,
                  "language_id": 3,
                  "image": "TourCity201405051399312413_5367d01d13d97.jpg"
                }
              }
            ],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "ownexpense",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "23",
                "tips": "",
                "ownexpense_description": {
                  "name": "洛杉矶自费景点2",
                  "description": "啥amy"
                }
              }
            ]
          },
          {
            "item_type": "hotel",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "rrrrrrrrrrrrrrrrrrrrrrrrrrrrrr",
                "description": "d",
                "image_url": "d"
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "transport",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 4,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "rge",
                "description": "ww",
                "image_url": "www"
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 2,
        "itinerary_no": 1,
        "mileage": "3.26",
        "tips": "为了给各位贵宾提供更高效贴心的服务，如果您下单并支付全额团费的日期距离您选择的出团时间在3天及以上，我们100%保证为您保留座位。",
        "has_city": 0,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 0,
        "has_attraction": 1,
        "summary": "早上继续畅游尼加拉大瀑布之旅，前往位于尼加拉河上的公羊岛，欣赏白天的大瀑布，更有机会看到挂在瀑布上的彩虹，之后到位于美国瀑布旁的电影院欣赏大瀑布IMAX电影*，在IMAX电影院内感受震撼的音响及超大银幕，作为游览尼加拉大瀑布的完美结局；之后前往下一城市波士顿，晚上到达位于麻省的波士顿，首先当然要先品尝当地最有名的波士顿龙虾*作为晚餐，大小适中的波士顿龙虾，爽口甜美，非吃不可！",
        "title": "纽约市博物馆-纽约唐人街",
        "itineraryItem": [
          {
            "item_type": "attraction",
            "order": 4,
            "attraction_item": [
              {
                "duration": "1.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "纽约市博物馆",
                  "pinyin": "N",
                  "alias": "",
                  "description": "",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 345,
                  "language_id": 3,
                  "image": "TourCity201405051399312413_5367d01d13d97.jpg"
                }
              }
            ],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "attraction",
            "order": 6,
            "attraction_item": [
              {
                "duration": "1.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "纽约唐人街",
                  "pinyin": "N",
                  "alias": "",
                  "description": "",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 106,
                  "language_id": 3,
                  "image": "chinatown_new_york.jpg"
                }
              }
            ],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "ownexpense",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "23",
                "tips": "",
                "ownexpense_description": {
                  "name": "洛杉矶自费景点2",
                  "description": "啥amy"
                }
              }
            ]
          },
          {
            "item_type": "ownexpense",
            "order": 2,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "140",
                "tips": "",
                "ownexpense_description": {
                  "name": "candy测试自费项目",
                  "description": "123344455"
                }
              }
            ]
          },
          {
            "item_type": "hotel",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "rg",
                "description": "rg",
                "image_url": "reg"
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "rge",
                "description": "rg",
                "image_url": "re"
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 3,
        "itinerary_no": 1,
        "mileage": "3.26",
        "tips": "为了给各位贵宾提供更高效贴心的服务，如果您下单并支付全额团费的日期距离您选择的出团时间在3天及以上，我们100%保证为您保留座位。",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 1,
        "has_attraction": 0,
        "summary": "早上继续畅游尼加拉大瀑布之旅，前往位于尼加拉河上的公羊岛，欣赏白天的大瀑布，更有机会看到挂在瀑布上的彩虹，之后到位于美国瀑布旁的电影院欣赏大瀑布IMAX电影*，在IMAX电影院内感受震撼的音响及超大银幕，作为游览尼加拉大瀑布的完美结局；之后前往下一城市波士顿，晚上到达位于麻省的波士顿，首先当然要先品尝当地最有名的波士顿龙虾*作为晚餐，大小适中的波士顿龙虾，爽口甜美，非吃不可！",
        "title": "2",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "比林斯",
                  "pinyin": "B",
                  "alias": "",
                  "description": ""
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "ownexpense",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "23",
                "tips": "",
                "ownexpense_description": {
                  "name": "洛杉矶自费景点2",
                  "description": "啥amy"
                }
              }
            ]
          },
          {
            "item_type": "ownexpense",
            "order": 2,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "140",
                "tips": "",
                "ownexpense_description": {
                  "name": "candy测试自费项目",
                  "description": "123344455"
                }
              }
            ]
          },
          {
            "item_type": "hotel",
            "order": 4,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "rg",
                "description": "rg",
                "image_url": "reg"
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "transport",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "rge",
                "description": "rg",
                "image_url": "re"
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 4,
        "itinerary_no": 1,
        "mileage": "3.26",
        "tips": "为了给各位贵宾提供更高效贴心的服务，如果您下单并支付全额团费的日期距离您选择的出团时间在3天及以上，我们100%保证为您保留座位。",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 1,
        "has_attraction": 0,
        "summary": "早上继续畅游尼加拉大瀑布之旅，前往位于尼加拉河上的公羊岛，欣赏白天的大瀑布，更有机会看到挂在瀑布上的彩虹，之后到位于美国瀑布旁的电影院欣赏大瀑布IMAX电影*，在IMAX电影院内感受震撼的音响及超大银幕，作为游览尼加拉大瀑布的完美结局；之后前往下一城市波士顿，晚上到达位于麻省的波士顿，首先当然要先品尝当地最有名的波士顿龙虾*作为晚餐，大小适中的波士顿龙虾，爽口甜美，非吃不可！",
        "title": "3",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "比林斯",
                  "pinyin": "B",
                  "alias": "",
                  "description": ""
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "ownexpense",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "23",
                "tips": "",
                "ownexpense_description": {
                  "name": "洛杉矶自费景点2",
                  "description": "啥amy"
                }
              }
            ]
          },
          {
            "item_type": "ownexpense",
            "order": 2,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "140",
                "tips": "",
                "ownexpense_description": {
                  "name": "candy测试自费项目",
                  "description": "123344455"
                }
              }
            ]
          },
          {
            "item_type": "hotel",
            "order": 4,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "rg",
                "description": "rg",
                "image_url": "reg"
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "transport",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "rge",
                "description": "rg",
                "image_url": "re"
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 5,
        "itinerary_no": 1,
        "mileage": "3.26",
        "tips": "为了给各位贵宾提供更高效贴心的服务，如果您下单并支付全额团费的日期距离您选择的出团时间在3天及以上，我们100%保证为您保留座位。",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 1,
        "has_attraction": 0,
        "summary": "早上继续畅游尼加拉大瀑布之旅，前往位于尼加拉河上的公羊岛，欣赏白天的大瀑布，更有机会看到挂在瀑布上的彩虹，之后到位于美国瀑布旁的电影院欣赏大瀑布IMAX电影*，在IMAX电影院内感受震撼的音响及超大银幕，作为游览尼加拉大瀑布的完美结局；之后前往下一城市波士顿，晚上到达位于麻省的波士顿，首先当然要先品尝当地最有名的波士顿龙虾*作为晚餐，大小适中的波士顿龙虾，爽口甜美，非吃不可！",
        "title": "4",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "比林斯",
                  "pinyin": "B",
                  "alias": "",
                  "description": ""
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "ownexpense",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "23",
                "tips": "",
                "ownexpense_description": {
                  "name": "洛杉矶自费景点2",
                  "description": "啥amy"
                }
              }
            ]
          },
          {
            "item_type": "ownexpense",
            "order": 2,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "140",
                "tips": "",
                "ownexpense_description": {
                  "name": "candy测试自费项目",
                  "description": "123344455"
                }
              }
            ]
          },
          {
            "item_type": "hotel",
            "order": 4,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "rg",
                "description": "rg",
                "image_url": "reg"
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "transport",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "rge",
                "description": "rg",
                "image_url": "re"
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 6,
        "itinerary_no": 1,
        "mileage": "3.26",
        "tips": "为了给各位贵宾提供更高效贴心的服务，如果您下单并支付全额团费的日期距离您选择的出团时间在3天及以上，我们100%保证为您保留座位。",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 1,
        "has_attraction": 1,
        "summary": "早上继续畅游尼加拉大瀑布之旅，前往位于尼加拉河上的公羊岛，欣赏白天的大瀑布，更有机会看到挂在瀑布上的彩虹，之后到位于美国瀑布旁的电影院欣赏大瀑布IMAX电影*，在IMAX电影院内感受震撼的音响及超大银幕，作为游览尼加拉大瀑布的完美结局；之后前往下一城市波士顿，晚上到达位于麻省的波士顿，首先当然要先品尝当地最有名的波士顿龙虾*作为晚餐，大小适中的波士顿龙虾，爽口甜美，非吃不可！",
        "title": "纽约市博物馆-纽约唐人街",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "Newark",
                  "pinyin": "N",
                  "alias": "",
                  "description": ""
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "attraction",
            "order": 2,
            "attraction_item": [
              {
                "duration": "1.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "纽约市博物馆",
                  "pinyin": "N",
                  "alias": "",
                  "description": "",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 345,
                  "language_id": 3,
                  "image": "TourCity201405051399312413_5367d01d13d97.jpg"
                }
              }
            ],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "ownexpense",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "23",
                "tips": "",
                "ownexpense_description": {
                  "name": "洛杉矶自费景点2",
                  "description": "啥amy"
                }
              }
            ]
          },
          {
            "item_type": "hotel",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "The Glendon Hotel \r\n Knights Inn",
                "description": "t",
                "image_url": "t"
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "transport",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 4,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "rge",
                "description": "ww",
                "image_url": "www"
              }
            ],
            "ownexpense_item": []
          }
        ]
      }
    ]
  }
}
```



