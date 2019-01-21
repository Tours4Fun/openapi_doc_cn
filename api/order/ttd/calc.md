# Product price calculation

### Description

    Get the product price for create order

### API address

    api_open/order/cal

### Request parameter description

| Parameter           | Type          | Is required  | Description             |
| ------------------- |:-------------:| ------------:| :-----------------------|
| product_id          | int           |     Yes      |   Product id         |
| departure_date      | date          |     Yes      |   Travel date          |
| tickets             | array         |     Yes      |   --|
| -sku_id             | int           |     Yes      |   Sku id|
| -count              | int           |     Yes      |   The number of sku purchases|

### Request parameter demo

	{
    		"product_id":102851716,
    		"departure_date":"2019-01-22",
    		"tickets":[
            	{
                   "sku_id":756,
                   "count":1
                },
                {
                   "sku_id":755,
                   "count":20
                }
            ]
    }	

### Return field description

| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| total_retail                      |     Product dollar price                             |
| currency                          |     Dollar code                                  |
| product                           |     --                             |
| -product_id                       |     Product id                              |
| -departure_date                   |     Departure date          |
| -currency                         |     Product currency code                            |
| -symbol                           |     Product currency symbol                            |
| -product_price                    |     Product Price                            |
| -detail                           |     --                            |
| --sku_id                          |     Sku id                            |
| --amount                          |     The number of sku purchases                            |
| --price                           |     The total price of this sku                            |
| --display_name                    |     Display name                            |
| --sku_name                        |     Sku name                            |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "total_retail": 503.0275,
            "currency": "USD",
            "product": {
                "product_id": 102851716,
                "departure_date": "2019-01-22",
                "currency": "EUR",
                "symbol": "€",
                "product_price": 432,
                "detail": [
                    {
                        "sku_id": 756,
                        "amount": 1,
                        "price": 12,
                        "display_name": "3c",
                        "sku_name": "Gale Side(酒店内侧,较为安静,提供双人标准间或大床房)|成人"
                    },
                    {
                        "sku_id": 755,
                        "amount": 20,
                        "price": 420,
                        "display_name": "2b",
                        "sku_name": "Freeway Side(靠近Freeway,相对会有噪音,仅提供双人标准间)|成人"
                    }
                ]
            }
        }
    }


