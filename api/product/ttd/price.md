# Product Price

### Description

    Get the product price

### API address

    api_open/product/price

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| returnFields        | array         |     No      |   If empty default["price", "month", "calendar"]         |
| productIds          | array         |     Yse     |   Product ids          |
| conditions          | array         |     No      |   price.currency currency code[default:product currency]; calendar.m calendar price month [default:Current month]; calendar.currency currency code[default:product currency]|

    Supported currency
| Currency                             |     Symbol                                   |
| -------------------               |  :-----------------------                         |
|USD | $|
|GBP | £|
|AUD | AUD|
|NZD | NZD|
|EUR | €|
|CAD | C$|
|CNY | ¥|
|HKD | HK$|
|RUB | руб|
|KRW | ₩|
|SUR | py6|
|JPY | ¥|
|ZAR | R|
|NOK | kr|
|PHP | ₱|
|SEK | kr|
|CHF | Fr|
|DKK | kr|
|AED | AED|

### Request parameter demo

	{
    	"returnFields":["price","month","calendar"],
    	"productIds":[102851680],
    	"conditions":{
    		"price":{"currency":"cny"},
    		"calendar":{"m":["2019-2"],"currency":"usd"}
    	}
    }

### Return field description

    price[Product display price]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| display_price                     |     Product display price, The lowest price of all sku in a year                             |
| currency                          |     Currency code                                  |
| symbol                            |     Currency symbol                             |
| sku                               |     --                              |
| -price                            |     Sku display price, The lowest price of sku in a year           |
| -sku_id                           |     SkuId                            |

    month[The month the product can be sold]
    
    calendar[Product price]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| date                              |     Date[Y-m-d]                             |
| display_price                     |     Price                                  |
| remaining                         |     Stock, Take the minimum of all sku on the day                              |
| status                            |     If it is empty, it can be sold on the same day.["","disabled","soldout"]                               |
| currency                          |     Currency code           |
| symbol                            |     Currency symbol                            |
| sku                               |     --                            |
| -price                            |     This sku price                       |
| -remaining                        |     Sku stock                            |
| -is_holiday_price                 |     Holiday price[1=>yes, 0=>no]                                 |
| -sku_id                           |     SkuId                            |
| -sku_name                         |     Sku Name                            |

### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "102851680": {
                "price": {
                    "display_price": 897.3954,
                    "currency": "CNY",
                    "symbol": "¥",
                    "sku": [
                        {
                            "price": 176.2741,
                            "sku_id": 553
                        },
                        {
                            "price": 24.0374,
                            "sku_id": 554
                        },
                        {
                            "price": 96.1495,
                            "sku_id": 555
                        },
                        {
                            "price": 176.2741,
                            "sku_id": 556
                        },
                        {
                            "price": 96.1495,
                            "sku_id": 557
                        },
                        {
                            "price": 352.5482,
                            "sku_id": 558
                        },
                        {
                            "price": 440.6853,
                            "sku_id": 559
                        }
                    ]
                },
                "calendar": [
                    {
                        "date": "2019-02-01",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-02",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-03",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-04",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-05",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-06",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-07",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-08",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-09",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-10",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-11",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-12",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-13",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-14",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-15",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-16",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-17",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-18",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-19",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-20",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-21",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-22",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-23",
                        "display_price": 3.4932,
                        "remaining": 2,
                        "status": "",
                        "currency": "USD",
                        "symbol": "$",
                        "sku": [
                            {
                                "price": 25.6171,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 553,
                                "display_name": "2b",
                                "sku_name": "时间:19:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 3.4932,
                                "remaining": 2,
                                "is_holiday_price": 0,
                                "sku_id": 554,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:120 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 555,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 25.6171,
                                "remaining": 3,
                                "is_holiday_price": 0,
                                "sku_id": 556,
                                "display_name": "",
                                "sku_name": "时间:15:00|时长:80 hours|test other|成人"
                            },
                            {
                                "price": 13.973,
                                "remaining": 4,
                                "is_holiday_price": 0,
                                "sku_id": 557,
                                "display_name": "哈哈",
                                "sku_name": "时间:19:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 51.2343,
                                "remaining": 5,
                                "is_holiday_price": 0,
                                "sku_id": 558,
                                "display_name": "aaa",
                                "sku_name": "时间:15:00|时长:120 hours|test other|儿童"
                            },
                            {
                                "price": 64.0429,
                                "remaining": 16,
                                "is_holiday_price": 0,
                                "sku_id": 559,
                                "display_name": "",
                                "sku_name": "时间:19:00|时长:80 hours|test other|儿童"
                            }
                        ]
                    },
                    {
                        "date": "2019-02-24",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-25",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-26",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-27",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    },
                    {
                        "date": "2019-02-28",
                        "display_price": "",
                        "remaining": "",
                        "status": "disabled",
                        "currency": "",
                        "symbol": "",
                        "sku": []
                    }
                ],
                "month": [
                    "2019-01",
                    "2019-02",
                    "2019-07",
                    "2020-01",
                    "2020-04"
                ]
            }
        }
    }


