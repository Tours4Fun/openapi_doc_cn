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
      "updated_at": 1491908403,
      "name": "(3天)美西休閑之旅：納帕谷品美酒、太浩湖賞湖光山色、優勝美地覽峰巒瀑布",
      "image_url": "http://dn-tffimg.qbox.me/df/26/ca5/126/7a3d8c11749e9db6b0e670.jpg",
      "advertised_price": "346.0000",
      "duration": "3.00",
      "duration_type": "day",
      "stock_status": 0,
      "max_child_age": 0,
      "min_days_before_departure": 0,
      "min_guest_number": 1,
      "display_itinerary_note": 1,
      "show_ownexpense": 1,
      "visa_passport": 0,
      "is_pickup": 0,
      "is_dropoff": 0,
      "product_id": 101561985,
      "product_line": "tour",
      "product_passenger": {
        "lastname_en": {
          "name": "lastname_en",
          "label": "姓氏",
          "type": "text",
          "min": "",
          "max": "",
          "options": [],
          "placeholder": "",
          "display_name_en": "Last Name"
        },
        "firstname_en": {
          "name": "firstname_en",
          "label": "名字",
          "type": "text",
          "min": "",
          "max": "",
          "options": [],
          "placeholder": "",
          "display_name_en": "First Name"
        },
        "mobile": {
          "name": "mobile",
          "label": "電話",
          "type": "phone",
          "min": "",
          "max": "",
          "options": [],
          "placeholder": "",
          "display_name_en": "Mobile"
        }
      },
      "departure_city_name": [
        {
          "departure_city_id": 2,
          "departure_city_name": "舊金山"
        },
        {
          "departure_city_id": 64,
          "departure_city_name": "聖何塞"
        },
        {
          "departure_city_id": 542,
          "departure_city_name": "舊金山灣區"
        }
      ],
      "return_city_name": [
        {
          "return_city_id": 2,
          "return_city_name": "舊金山"
        },
        {
          "return_city_id": 64,
          "return_city_name": "聖何塞"
        },
        {
          "return_city_id": 542,
          "return_city_name": "舊金山灣區"
        }
      ],
      "region_chinese_name": "美國",
      "region": "us",
      "sub_region_chinese_name": "美西",
      "sub_region": "west",
      "base_price": {
        "single": 428,
        "double": 346,
        "triple": 293,
        "quad": 247,
        "kid": 0
      }
    },
    "info": {
      "brief_description": "★ 前往納帕酒鄉欣賞田園美景，還可自費品嘗絕世佳釀，盡享悠閑的浪漫時光<br>\r\n★ 置身於太浩湖絕美的湖光山色之中，湖水藍如寶石，四周群山環繞，仿佛置身天外仙境<br>\r\n★ 游覽美西最負盛名的優勝美地國家公園，遙望懸崖峭壁、千丈飛瀑，別有一番趣味<br>",
      "full_description": "",
      "airport_transfer_info": "",
      "notice": "* 所有旅客必須在出發前30分鍾到達指定的上車地點。所有旅客必須憑上車許可，團票或在線預定時的確認號上車。<br>\r\n* 網上預訂後，您將會收到一封“確認郵件”（電子票），內附完整的使用說明，包括目的地的當地電話等。當您確定後，請務必打印該“確認郵件”（電子票），並在旅途中隨身攜帶——這是您已付款的證據。<br>\r\n* 為改進線路，提高可操作性，或因不可抗力，有必要更改線路時，我們有權改變行程和住宿酒店。旅游旺季時期，或將增派車輛保證滿足需求。<br><br>",
      "includes": "* 豪華大巴接送<br>\r\n* 兩晚酒店住宿，所有酒店提供雙人床，標准間<br>\r\n* 精心安排旅館酒店及大型巴士，讓您的旅程舒適又安全<br>\r\n* 當地最具經驗的專職雙語導游(半自助導游)和駕駛經驗豐富的車長<br>",
      "excludes": "<LI>不提供您往返出發地和舊金山機場或指定接客地點的機票和相關交通費用</LI>\r\n<LI>不包括提供給導游和司機的服務費（每位客人支付司機及導游服務費：共$8.00/每天）</LI>\r\n<LI>所有個人費用(洗衣服，電話費，餐費和個人保險等)，行程中的門票或自費項目(自費項目和價格可能會因為季節變化而有所調整，最終請以出團當天的實際項目和售票窗口的實際價格為准)</LI>",
      "package_special_note": "",
      "price_special_note": "* 單人間價格是指一人單獨享有一個酒店標准間的價格。<br>\r\n* 雙人/三人/四人間是指雙人/三人/四人共同享用一個酒店標准間的價格。<br>\r\n* 三人/四人間價格不包括在房間里另加床位的價格，另加床位要在登記時單獨提出要求。<br>\r\n* 請注意：由於酒店標准間空間及所加床位有限，請客人自行向酒店服務台咨詢加床事宜，途風不能保證加床成功。<br>\r\n* 小孩與成人同價。 <br>\r\n* 一個房間最多只能容納包括成人和小孩或嬰兒在內共四人。<br>\r\n@@<FONT color=#f7860f><p align=\"left\" class=\"STYLE5\">團購活動價格說明：</p>\r\n<p align=\"left\" class=\"STYLE5\">*進行團購活動的行程享受途風團購低價保證服務；</p>\r\n<p align=\"left\" class=\"STYLE5\">*如果您選擇的出團日期為假日價格，將不能享受團購優惠，請您悉知；</p>\r\n<p align=\"left\" class=\"STYLE5\">*以團購價格預訂的行程，在團購活動結束後，修改訂單信息(變更出團日期或人數)，將按照最新的價格進行計算，不享受團購優惠。</p>@@</FONT>",
      "eticket_special_note": "***【參團須知】***\r\n* 為確保您的行程順利，請您在出發前一天務必致電給途風獲取並確認領隊的聯絡方式。\r\n* 支付給導游和司機的服務費以及團費不包括中的自費項目費用將會以現金方式收取，參團前請您把這部分費用計劃在旅行開支內。\r\n\r\n***【其他說明】***\r\n* 請注意：對於當地地接巴士部門的軟性服務，或由於天氣、交通、航班臨時取消等不可預計的突發狀況而臨時被迫更改行程的出發時間，或游覽車出現臨時故障而被迫取消部分游覽景點等不可控制因素，途風首先保留為客人爭取最高權益的義務和責任，但最終解釋權由地接巴士部決定。\r\n* 在出行中，請旅客尊重領隊及司機的工作，按照美國旅游交通法律規定，對於在行程中刻意以各種方式影響行程進行，導致產生不良後果的舉動，巴士地接社有權使用法律手段立即終止旅客的行程，此行為與途風無關。\r\n* 為保障您的個人財產安全，我們建議您在旅行期間隨身攜帶個人貴重物品，不要將貴重物品遺留在大巴/酒店/景點/餐館等地點；在任何情況及任何地點下失竊，造成個人財產損失，途風、地接社及司機、領隊導游等均不負任何責任，請您悉知。",
      "tips": "",
      "additional_promotion": "",
      "credential": "",
      "change_notice": "離出發日(不含當天)超過17天，退還費用的75%；<br>\r\n離出發日(不含當天)10-16天，退還費用的50%；<br>\r\n離出發日(不含當天)6-9天，退還費用的25%；<br>\r\n離出發日(不含當天)5天之內，不退還任何費用。<br>\r\n* 除以上罰金之外，還將收取6%的手續費。<br>\r\n* 所有景點門票，城市通票等不可更改或退款。<br>\r\n* 每位旅客需要在預定時付全款，如缺席或在中途提前離開，將被視作自動放棄，恕不退款。<br>\r\n* 旅客必須在退款時出示團票。<br>\r\n* 我們有權因人數不達要求取消行程並作出全額退款。我們承諾盡最大努力確保旅行按計劃實行。<br>",
      "auto_confirm": "",
      "travel_notice": "* 在旺季期間，由於酒店房間供應緊張，我們可能會為您更換同等級的酒店，謝謝您的理解及支持！",
      "product_tips": ""
    },
    "language": [
      {
        "language_type": "live",
        "name": "中文 Live",
        "icon": "chinese_live.jpg",
        "sort_order": 1
      },
      {
        "language_type": "live",
        "name": "英語 Live",
        "icon": "english_live.jpg",
        "sort_order": 0
      }
    ],
    "itinerary": [
      {
        "day_no": 1,
        "itinerary_no": 1,
        "mileage": "0.00",
        "tips": "",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 0,
        "has_transport": 0,
        "has_attraction": 1,
        "summary": "參觀位於納帕酒鄉的美麗酒庄，您可自費品嘗各式香醇美酒。納帕酒庄的田園美景和充足的藏酒讓人不由得放慢腳步，駐足細細品味絕世佳釀。釀酒廠擁有氣派的建築物，配搭充滿古典色彩的古董家具。每個角落都洋溢着悠閑的浪漫時光。下午我們來到加州首府薩克拉門托參觀游覽。我們將在雷諾住宿一晚，您可以探索賭場和夜總會。\r\n\r\n<font color=\"#FF6600\"><b>納帕谷葡萄酒品嘗：</b></font>\r\n令人驚嘆的自然之美留出這一地區，生產世界上最好的葡萄酒。擁有更多的世界著名釀酒廠，95%的納帕谷酒廠，400余家酒廠都是家族擁有和經營。 \r\n可選擇不同的酒廠品酒，價格不一，以實際為准。\r\n\r\n<font color=\"#FF6600\"><b>薩克拉門托(Sacramento)：</b></font>\r\n加州州議會大廈(California State Capitol)，同時也作為博物館和美國的政府工作大樓，常年向公眾開放，供游客參觀了解加州的豐富歷史，大廈也見證了現代憲法立法的整個進程。",
        "title": "舊金山(San Francisco) - 納帕酒鄉(Napa Valley) - 薩克拉門托(Sacramento) - 雷諾(Reno)",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "舊金山",
                  "pinyin": "J",
                  "alias": "",
                  "description": "舊金山，又譯“聖弗朗西斯科”、“三藩市”。舊金山是美國加利福亞州太平洋沿岸港口城市，加州僅次於洛杉磯的第二大城市，美國西部最大的金融中心和重要的高新技術研發和制造基地，位於美國西海岸，太平洋與聖弗朗西斯科灣之間的半島北端。舊金山是美洲華人最為密集的聚居地，也是世界上著名的高新技術產業園“硅谷”的所在地，每天吸納着無數高科技人才和世界各地的游人。"
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "city",
            "order": 2,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "薩克拉門托",
                  "pinyin": "S",
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
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "雷諾",
                  "pinyin": "L",
                  "alias": "",
                  "description": "雷諾（RENO）享有“全世界最大的小城市”之稱。這里是美國最老的賭城之一，也被評為”全美最適合居住的十大城市”之一。欣賞七彩艷麗的霓虹燈，享受多彩多姿的夜生活，所有的一切，應有盡有。雷諾（RENO）是一個充滿着生機的城市，其中的博物館、藝術畫廊、國家公園、都被當地的居民和旅客視為世界一流的文化及室外活動盛行的度假勝地。加上每年有300多天的陽光普照，RENO吸引着成千上萬的旅客。20世紀上半葉，離婚不像現在這樣普遍和自由，而且離婚是不光彩的事。但是在雷諾，有一種“無責任離婚”，離婚無需理由，只要住夠規定的時間，交一定的費用就可離婚。所以，成千上萬的美國人為了順利離婚而蜂擁至此，使這個城市名噪一時。"
                }
              }
            ],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "attraction",
            "order": 4,
            "attraction_item": [
              {
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "納帕谷(酒鄉)",
                  "pinyin": "N",
                  "alias": "",
                  "description": "納帕山谷位於美國加利福亞州北部，是一片廣袤綿延的丘陵。納帕山谷陽光燦爛，氣候宜人，清澈的溪水靜靜地流淌，滋潤着兩岸翡翠般的草地和溝壟線條流暢的葡萄園，同時醞釀出醇香柔和回味無窮的納帕葡萄酒。納帕是美國最優秀的葡萄酒產區之一，主要釀制紅葡萄酒、白葡萄酒、香檳等，是世界第四大葡萄酒產地，已經成為美國酒文化的代名詞，新世紀葡萄酒行業高貴典雅的品質象征。  帕酒庄的田園美景和充足的藏酒讓你不由得放慢腳步，駐足細細品味絕世佳釀。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 24,
                  "language_id": 3,
                  "image": "https://d3ne5s9fv9p81l.cloudfront.net/images/Ripe_grapes_napa_valley.jpg"
                }
              }
            ],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "hotel",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "Reno Sands Casino Hotel ",
                "description": "",
                "image_url": ""
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "餐食：自理",
                "description": "",
                "image_url": ""
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 2,
        "itinerary_no": 1,
        "mileage": "0.00",
        "tips": "",
        "has_city": 1,
        "has_hotel": 1,
        "has_meal": 1,
        "has_ownexpense": 1,
        "has_transport": 0,
        "has_attraction": 1,
        "summary": "早晨我們將出發前往太浩湖。太浩湖是橫跨美國加州和內華達州的大淡水湖泊，海拔 6,225 英尺 (1,897 m)，由附近雪山融雪積水而成，所以湖水終年冰涼清澈，是美國第二深的高山湖泊，也是加州大部分民眾的度假首選。",
        "title": "雷諾(Reno) - 太浩湖(Lake Tahoe) - 特雷西(Tracy)",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "雷諾",
                  "pinyin": "L",
                  "alias": "",
                  "description": "雷諾（RENO）享有“全世界最大的小城市”之稱。這里是美國最老的賭城之一，也被評為”全美最適合居住的十大城市”之一。欣賞七彩艷麗的霓虹燈，享受多彩多姿的夜生活，所有的一切，應有盡有。雷諾（RENO）是一個充滿着生機的城市，其中的博物館、藝術畫廊、國家公園、都被當地的居民和旅客視為世界一流的文化及室外活動盛行的度假勝地。加上每年有300多天的陽光普照，RENO吸引着成千上萬的旅客。20世紀上半葉，離婚不像現在這樣普遍和自由，而且離婚是不光彩的事。但是在雷諾，有一種“無責任離婚”，離婚無需理由，只要住夠規定的時間，交一定的費用就可離婚。所以，成千上萬的美國人為了順利離婚而蜂擁至此，使這個城市名噪一時。"
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
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "太浩湖",
                  "pinyin": "T",
                  "alias": "",
                  "description": "太浩湖又譯作塔霍湖，是一個位於美國加利福亞州和內華達州邊界上的湖泊，在內華達州首府卡森城以西約10英里的地方。它是北美最大的高山湖泊。深501米，是美國第二深的湖泊。湖泊蓄水量為150.68249立方千米，蓄水量全世界排名第26位。海拔1897米。太浩湖是一個兩座山脈間斷層移動陷落所造成的大湖，有多座山頭圍繞湖邊，因此冬天是絕佳的滑雪場，夏天則是避暑勝地。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 552,
                  "language_id": 3,
                  "image": "https://d3ne5s9fv9p81l.cloudfront.net/images/lake_tahoe_california.jpg"
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
            "order": 3,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": [
              {
                "price": "$59.00/成人；$29.00/小孩(3-11歲)；$59.00/老人",
                "tips": "",
                "ownexpense_description": {
                  "name": "太浩湖巡航",
                  "description": ""
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
                "name": "Days Inn",
                "description": "",
                "image_url": ""
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "hotel",
            "order": 5,
            "attraction_item": [],
            "hotel_item": [
              {
                "name": "Similar Nearby Tracy",
                "description": "",
                "image_url": ""
              }
            ],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 6,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "餐食：自理",
                "description": "",
                "image_url": ""
              }
            ],
            "ownexpense_item": []
          }
        ]
      },
      {
        "day_no": 3,
        "itinerary_no": 1,
        "mileage": "0.00",
        "tips": "",
        "has_city": 1,
        "has_hotel": 0,
        "has_meal": 1,
        "has_ownexpense": 0,
        "has_transport": 0,
        "has_attraction": 1,
        "summary": "游覽美西最負盛名的優勝美地國家公園，一路怪石嶙峋、懸崖峭壁、千丈飛瀑、萬里峰巒、仿彿罝身世外。公園內著名景致區如下：新娘面紗瀑布、船長巨岩、昆仲斜岩石、金沙江、觀瀑橋、半球巨岩、斷層飛瀑、南眺景等。游畢返回灣區。\r\n\r\n<font color=\"#FF6600\">隧道觀景點(Tunnel View)</font> 優勝美地有名的景點之一。它像一幅優勝美地的預覽，從那里可以看到船長岩、新娘的面紗、半圓丘等著名的優勝美地景點。 \r\n<font color=\"#FF6600\">新娘面紗瀑布(Bridal Veil Falls)</font> 高620英尺，是公園第2大瀑布，朦朦朧朧的像一塊新娘面紗一般懸在空中。它是優勝美地國家公園的五大瀑里，知名度相當高的瀑布。 \r\n<font color=\"#FF6600\">船長岩(El Capitan)</font> 又稱“酋長巨石”。它是優勝美地最有知名度的景點之一。酋長巨石高3000英尺(910公尺)，如果以一層樓3公尺計算，它的高度約為303層樓高。 \r\n<font color=\"#FF6600\">默塞德河(Merced River)</font> 默塞德河淌過華達州和優勝美地國家公園的瀑布。河流蜿蜒穿過優勝美地國家公園山谷，匯聚成一條清澈的河流。 \r\n<font color=\"#FF6600\">優勝美地瀑布(Yosemite Falls)</font> 優勝美地瀑布是北美最高的瀑布，是優勝美地谷最強大的組成部分。不論春夏秋冬季節如何變化，這個宏偉的瀑布一直是一個充滿活力的動力。 \r\n<font color=\"#FF6600\">半圓丘(Half Dome)</font> 表面受冰河作用切割的很平，像刀削的似的，矗立於海拔8842英尺的頂峰上，是優勝美地最高的山峰。也是世界最具挑戰性的攀岩地之一。\r\n若您准備當天飛離舊金山，建議預訂11:00pm之後的航班。\r\n",
        "title": "優勝美地(Yosemite) - 舊金山(San Francisco)",
        "itineraryItem": [
          {
            "item_type": "city",
            "order": 1,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [
              {
                "city_description": {
                  "name": "舊金山",
                  "pinyin": "J",
                  "alias": "",
                  "description": "舊金山，又譯“聖弗朗西斯科”、“三藩市”。舊金山是美國加利福亞州太平洋沿岸港口城市，加州僅次於洛杉磯的第二大城市，美國西部最大的金融中心和重要的高新技術研發和制造基地，位於美國西海岸，太平洋與聖弗朗西斯科灣之間的半島北端。舊金山是美洲華人最為密集的聚居地，也是世界上著名的高新技術產業園“硅谷”的所在地，每天吸納着無數高科技人才和世界各地的游人。"
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
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "優勝美地國家公園",
                  "pinyin": "Y",
                  "alias": "",
                  "description": "優勝美地國家公園位於加利福亞州東部內華達山脈上，是美國西部最美麗、參觀人數最多的國家公園之一，與大峽谷國家公園、黃石國家公園齊名。公園以優勝美地溪谷為中心，峽谷內有默塞德河流過，以及一些瀑布，包括著名的優勝美地瀑布。景觀中還有許多美麗的山峰，其中最著名的是船長峰，這是一個由谷底垂直向上高達1099米的花崗岩壁，是世界上最高的不間斷陡崖之一。公園內的地勢落差極大，不斷映入眼簾的山峰、峽谷、河流、瀑布，構成了山谷內鬼斧神工的雄偉景色。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 51,
                  "language_id": 3,
                  "image": "https://d3ne5s9fv9p81l.cloudfront.net/images/TourCity201606131465808363_575e75eb2981e.jpg"
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
            "order": 3,
            "attraction_item": [
              {
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "優勝美地新娘面紗瀑布",
                  "pinyin": "Y",
                  "alias": "",
                  "description": "新娘面紗瀑布 (Bridal Veil Falls) 高620英尺，是優勝美地國家公園里的第二大瀑布，朦朦朧朧的像一塊新娘面紗一般懸在空中。它是優勝美地國家公園的五大瀑里，知名度相當高的瀑布。5月份是觀賞瀑布的最佳時間，那時候高山上的雪水融化，瀑布的水量最足，夏天和秋天就會出像斷流的現象，而冬天有可能在瀑布口凍成冰凌。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 23113,
                  "language_id": 3,
                  "image": "TourCity201407111405106721_53c03a21e9409.jpg"
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
            "order": 4,
            "attraction_item": [
              {
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "船長岩",
                  "pinyin": "C",
                  "alias": "",
                  "description": "船長岩是世界上最險峻的峭壁之一，由極為堅硬且毫無裂紋的花崗岩形成，因此，強大的自然侵蝕似乎對它沒產生什么影響。船長岩是優勝美地的地標式景觀，從山谷谷底到船長岩頂部的距離為1100米，陡峭無比，岩壁光滑，異常險峻，從而吸引了世界各地專業攀岩者來挑戰。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 23116,
                  "language_id": 3,
                  "image": "TourCity201606131465808738_575e7762b2c16.jpg"
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
            "order": 5,
            "attraction_item": [
              {
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "半圓頂",
                  "pinyin": "B",
                  "alias": "",
                  "description": "Half Dome，直譯為“半圓頂”，是一塊半球形的巨大花崗岩山。它是美國加州Yosemite優山美地國家公園的象征，更是The North Face品牌logo的來源。Half Dome海拔近3000米，是優山美地里最高的山峰，比周圍山峰高出近1000米，所以當夕陽落下地平線，大地陷入陰影里的時候，Half Dome光滑的山壁獨自在夕陽下熠熠生輝，非常壯觀。Half Dome的西北壁是長約六百米，斜度達93%的垂直面，是世界上最具挑戰性的攀岩地之一，Yosemite優山美地國家公園也因此吸引了大量世界各地的專業攀岩者。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 23122,
                  "language_id": 3,
                  "image": "https://d3ne5s9fv9p81l.cloudfront.net/images/TourCity201407111405106767_53c03a4f10360.jpg"
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
                "duration": "0.0",
                "duration_type": "day",
                "is_optional": 0,
                "city_description": {
                  "name": "優勝美地瀑布",
                  "pinyin": "Y",
                  "alias": "",
                  "description": "優勝美地瀑布，是北美洲落差最大的瀑布，位於美國加州謝拉內華達山區，屬於優勝美地國家公園，其最壯觀的季節在春末，水量充沛，氣勢驚人。優勝美地瀑布全高為739公尺，一共可分為三段，瀑布的落差距離排名世界第六，雖然在外觀看來僅有上優勝美地瀑布與下優勝美地瀑布兩段，但事實上包括了中間的落差地帶，這三段分別是：上優勝美地瀑布、湍流區、下優勝美地瀑布。",
                  "transportation": "",
                  "languages": "",
                  "feature_foods": "",
                  "religious_culture": "",
                  "tips": "",
                  "operate_tips": "",
                  "tour_city_id": 23161,
                  "language_id": 3,
                  "image": "https://d3ne5s9fv9p81l.cloudfront.net/images/TourCity201407111405106672_53c039f0b391d.jpg"
                }
              }
            ],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 7,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [],
            "ownexpense_item": []
          },
          {
            "item_type": "meal",
            "order": 7,
            "attraction_item": [],
            "hotel_item": [],
            "city_item": [],
            "meal_item": [
              {
                "name": "餐食：自理",
                "description": "",
                "image_url": ""
              }
            ],
            "ownexpense_item": []
          }
        ]
      }
    ],
    "images": [
      {
        "url": "201605021462210141_57278e5dc2657_watermark_800_800.jpg"
      },
      {
        "url": "201605021462210250_57278ecab3204_watermark_800_800.jpg"
      },
      {
        "url": "http://dn-tffimg.qbox.me/21/45/c98/b26/fb800629487bc3cee38931.jpg"
      },
      {
        "url": "http://dn-tffimg.qbox.me/27/bf/3fa/628/86cc9c98e562763b74fe92.jpg"
      },
      {
        "url": "http://dn-tffimg.qbox.me/95/8b/f8c/342/6614a7ff15cd2544cdde2d.jpg"
      },
      {
        "url": "http://dn-tffimg.qbox.me/df/26/ca5/126/7a3d8c11749e9db6b0e670.jpg"
      }
    ]
  }
}
```
