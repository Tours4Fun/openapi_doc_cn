# Order List

### Description

    Get the order list

### API address

    api_open/order/list

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| page                | int           |     No      |   Page page number[default:1]         |
| page_size            | int           |     No      |   Number of paged data[default:10]          |

### Request parameter demo

	{
    	"page":1,
    	"page_size":20
    }

### Return field description

| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| order_id                          |     Order id                             |
| created_at                        |     Order create time                                  |
| updated_at                        |    Order modify time                            |
| currency                          |     Currency                              |
| price                             |     Order amount           |
| product_list                      |     Order related products                            |
| -product_id                       |     Product id               |
| -product_name                     |     Product name                                |
| -departure_date                   |     Travel time                           |
| -end_date                         |     Travel end time                                |
| -price_info                       |     --                                            |
| --total_retail                    |     Total amount of this product                                  |
| --currency                        |     Product currency                                  |
| --symbol                          |     Currency symbol                                   |
| -contact                          |     --                                            |
| --firstname                       |     First name                                  |
| --lastname                        |     Last name                                  |
| --telephone                       |     Telephone                                  |
| --email                           |     Email                                            |
| -detail                           |     Product sku detail                                  |
| --sku_id                          |     Sku id                                  |
| --amount                          |     Purchase quantity                      |
| --price                           |     The total price of this sku                      |
| --display_name                    |     Display name                      |
| --sku_name                        |     Sku name                      |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "cur_page": 1,
            "page_size": 20,
            "total_page": 1,
            "total_num": 2,
            "order_list": [
                {
                    "order_id": 10004051,
                    "created_at": "2019-01-21 14:34:36",
                    "updated_at": "2019-01-21 14:34:38",
                    "currency": "USD",
                    "price": 15.7672,
                    "product_list": [
                        {
                            "product_id": 102851724,
                            "product_name": "123123",
                            "departure_date": "2019-01-22",
                            "end_date": "2019-01-22",
                            "price_info": {
                                "total_retail": 22,
                                "currency": "AUD",
                                "symbol": "AUD"
                            },
                            "contact": {
                                "firstname": "Sagar",
                                "lastname": "Thesia",
                                "telephone": "9574775177",
                                "email": "sagart.bipl@gmail.com"
                            },
                            "detail": [
                                {
                                    "sku_id": 760,
                                    "amount": 1,
                                    "price": 11,
                                    "display_name": "666",
                                    "sku_name": "成人"
                                },
                                {
                                    "sku_id": 761,
                                    "amount": 1,
                                    "price": 11,
                                    "display_name": "999",
                                    "sku_name": "儿童"
                                }
                            ]
                        }
                    ]
                },
                {
                    "order_id": 10004052,
                    "created_at": "2019-01-21 16:25:22",
                    "updated_at": "2019-01-21 16:25:23",
                    "currency": "USD",
                    "price": 15.7672,
                    "product_list": [
                        {
                            "product_id": 102851724,
                            "product_name": "123123",
                            "departure_date": "2019-01-22",
                            "end_date": "2019-01-22",
                            "price_info": {
                                "total_retail": 22,
                                "currency": "AUD",
                                "symbol": "AUD"
                            },
                            "contact": {
                                "firstname": "Sagar",
                                "lastname": "Thesia",
                                "telephone": "9574775177",
                                "email": "sagart.bipl@gmail.com"
                            },
                            "detail": [
                                {
                                    "sku_id": 760,
                                    "amount": 1,
                                    "price": 11,
                                    "display_name": "666",
                                    "sku_name": "成人"
                                },
                                {
                                    "sku_id": 761,
                                    "amount": 1,
                                    "price": 11,
                                    "display_name": "999",
                                    "sku_name": "儿童"
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    }


