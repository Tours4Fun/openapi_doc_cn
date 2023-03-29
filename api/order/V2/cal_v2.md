# Price calculate

**Description**

Calculate the price of the order based on the room, guest number, and upgrade items selected by the user.

### API URL

    POST   /v2/order/cal

**Parameters**

| parameter           | type         | required | description             |
| -------------- |:-------------:| ----:| -----------------:|
| product_id    | integer  |  yes   | product ID   |
| departure_date      | string  |  yes   | departure date |
| departure_address   |string   |  yes   | departure address |
| upgrades            | array   |  yes   | upgrades（upgrade ID:upgrade item ID）|
| rooms              | array   |  yes   | room info|
| --adult            | integer |  yes   | adult number |
| --kid              | integer |  yes   | kid number |
| --single_pairup    | integer |  no   | is single paireup, yes or no |

**Reqeust parameter example**

```
{
    "product_id":102202692,
    "departure_date":"2019-01-16",
    "departure_address":"jhjhj",
    "upgrades":{
        "30100":["30577"]
    },
    "rooms":[
        {
            "adult":2,
            "kid":0,
            "single_pairup":0
        }
    ]
}
```
**Response**

```
{
    "product_id" => 102202692
    "product_line" => "activity"
    "currency" => "EUR"
    "total_retail" => 61.6
    "total_retail_target_currency" => 71.728
    "original_total_retail" => 80
    "original_total_retail_target_currency" => 93.1532
    "total_discount" => 18.4
    "total_discount_target_currency" => 21.4252
    "product_price_detail" => array:2 [
        "base_price" => array:3 [
            "total_retail" => 61.6
            "original_total_retail" => 80
            "base_price_detail" => array:1 [
                0 => array:4 [
                    "total_retail" => 61.6
                    "total_retail_target_currency" => 71.728
                    "original_total_retail" => 80
                    "original_total_retail_target_currency" => 93.1532
                ]
            ]
        ],
        "upgrades_price" => array:3 [
            "total_retail" => 0
            "total_retail_target_currency" => 0
            "upgrades_detail" => array:1 [
                30100 => array:4 [
                    "total_retail" => 0
                    "total_retail_target_currency" => 0
                    "upgrade_name" => "座位等级"
                    "upgrades_sub_detail" => array:1 [
                        0 => array:4 [
                            "option_id" => 30577
                            "total_retail" => 0
                            "total_retail_target_currency" => 0
                            "upgrade_sub_name" => "一等(First Class-Max.2 passengers)"
                        ]
                    ]
                ]
            ]
        ]
    ]
}
```
