# Product Price

### Description

    Get the product price

### API address

    ttd/product/price

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| product_ids         | array        |     Yse     |   Product ids          |
| currency            | string         |     No      |  currency code[default:USD] |

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
    	"product_ids":[102851680],
    	"currency":"cny"
    }

### Return field description

    price[Product departure time & price]
| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| timestamp                         |        timestamp                          |
| date                              |     date                                  |
| sku_id                            |     sku_id                             |
| price                             |     sku price                              |
| remaining                         |     sku stock           |
| is_holiday_price                  |     holiday price[1 => yes, 0 => no]                            |
| currency                          |     currency                            |
| symbol                            |     currency symbol                            |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "102851680": [
                {
                    "timestamp": 1548518400,
                    "date": "2019-01-27",
                    "sku_id": 553,
                    "price": 616.9594,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548518400,
                    "date": "2019-01-27",
                    "sku_id": 554,
                    "price": 216.3364,
                    "remaining": 1,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1548864000,
                    "date": "2019-01-31",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549555200,
                    "date": "2019-02-08",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1549728000,
                    "date": "2019-02-10",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550073600,
                    "date": "2019-02-14",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550160000,
                    "date": "2019-02-15",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550246400,
                    "date": "2019-02-16",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550678400,
                    "date": "2019-02-21",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550764800,
                    "date": "2019-02-22",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 553,
                    "price": 176.2741,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 554,
                    "price": 24.0374,
                    "remaining": 2,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 555,
                    "price": 96.1495,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 556,
                    "price": 176.2741,
                    "remaining": 3,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 557,
                    "price": 96.1495,
                    "remaining": 4,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 558,
                    "price": 352.5482,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1550851200,
                    "date": "2019-02-23",
                    "sku_id": 559,
                    "price": 440.6853,
                    "remaining": 16,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1562688000,
                    "date": "2019-07-10",
                    "sku_id": 554,
                    "price": 176.2741,
                    "remaining": 12,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1562860800,
                    "date": "2019-07-12",
                    "sku_id": 554,
                    "price": 176.2741,
                    "remaining": 12,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1563292800,
                    "date": "2019-07-17",
                    "sku_id": 554,
                    "price": 176.2741,
                    "remaining": 12,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1563811200,
                    "date": "2019-07-23",
                    "sku_id": 554,
                    "price": 176.2741,
                    "remaining": 12,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1578240000,
                    "date": "2020-01-06",
                    "sku_id": 554,
                    "price": 48.0748,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1578326400,
                    "date": "2020-01-07",
                    "sku_id": 554,
                    "price": 48.0748,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1578844800,
                    "date": "2020-01-13",
                    "sku_id": 554,
                    "price": 48.0748,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1578931200,
                    "date": "2020-01-14",
                    "sku_id": 554,
                    "price": 48.0748,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1579017600,
                    "date": "2020-01-15",
                    "sku_id": 554,
                    "price": 48.0748,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                },
                {
                    "timestamp": 1579190400,
                    "date": "2020-01-17",
                    "sku_id": 554,
                    "price": 48.0748,
                    "remaining": 5,
                    "is_holiday_price": 0,
                    "currency": "CNY",
                    "symbol": "¥"
                }
            ]
        }
    }


