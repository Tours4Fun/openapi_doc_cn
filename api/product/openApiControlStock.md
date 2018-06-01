### restore or reduce control stock.
According to the field 'use_control_stock'
to determine whether the operation is reduce or returned.If use_control_stock is 1,
it will be restore first and then consume,else it will only be restore
POST /control_stock/reduceOrRestore
```
params:
order_id   # order number(must param)
created_time   # order creation time(must param)
order_product_id    # order product ID(not must param,default 0)
product_id    # Product ID, new ID(must param)
departure_date    # Departure time(must param)
room_num    # Number of rooms(must param)
people    # number of people(must param)
distributor_id    # distribution id.If value = 0,it`s TFF or T4f or T4FES order.If value > 0,it`s distribution order(must param)
use_control_stock    # when the value is 1 that will be restore and then consume, when the value is 0 that will only be restore.So if you need consume you shound use_control_stock=1(must param)
store_id  # store id(must param)

Give an example with params
{
    "order_id":10010428,
    "created_time":"2018-03-29",
    "order_product_id":12827,
    "product_id":101818154,
    "departure_date":"2018-04-01",
    "room_num":3,
    "people":3,
    "distributor_id":0,
    "use_control_stock":1,
    "store_id":3
}

response:
{
    "code": 0,
    "message": "successful",
    "data": {
        "101818154": {
            "consumed": 1,
            "product_line": "tour",
            "message": "需要消耗3人/3房;\n        实际消耗本仓库2人/3房.\n        实际消耗公共仓库1人/0房.",
            "reduced_people": 1,   # reduced public stock with people
            "reduced_house": 0,   # reduced public stock with room
            "reduced_distribution_people": 2,   # reduced distribution stock with people
            "reduced_distribution_house": "3",   # reduced distribution stock with room
            "need_reduce_people": "3",   # The number of people actually needed to consume
            "need_reduce_house": "3"    # The number of room actually needed to consume
        }
    }
}
```

### get control stock by product_id and departure_date.
POST /control_stock/getControlStock
```
params:
order_id   # order number(must param)
order_product_id    # order product ID(not must param,default 0)
product_id    # Product ID, new ID(must param)
departure_date    # Departure time(must param)
store_id  # store id(must param)

{
    "order_id":10010428,
    "order_product_id":12827,
    "product_id":101818154,
    "departure_date":"2018-04-01",
    "store_id":3
}

response:
{
    "code": 0,
    "message": "",
    "data": {
        "control_stock_rule": [
            {
                "stock_id": 2,
                "stock_name": "工单测试",
                "stock_people_num": 20, # public stock with people
                "stock_house_num": 44,  # public stock with room
                "allocation_config": {  # distribution stock message
                    "1": {
                        "people": 0,
                        "house": 7,
                        "day": 4,
                        "name": "主站TFF"
                    },
                    "542211": {
                        "people": 13,
                        "house": 12,
                        "day": 3,
                        "name": "携程"
                    },
                    "1344606": {
                        "people": 20,
                        "house": 10,
                        "day": 4,
                        "name": "飞猪"
                    },
                    "3447396": {
                        "people": 37,
                        "house": 24,
                        "day": 3,
                        "name": "携程自由行定制"
                    }
                },
                "departure_date": "2018-04-01 00:00:00",
                "stock_start_date": "2018-03-20 00:00:00",
                "stock_end_date": "2018-04-04 00:00:00",
                "share_product_ids": "101818154,101576430",
                "total_people": 90,
                "total_house": 97
            }
        ],
        "reduce_log": {  # The latest consumption log
            "stock_id": 2,
            "stock_name": "工单测试",
            "stock_departure_date": "2018-04-01 00:00:00",
            "stock_people_change": "1",
            "stock_house_change": "0",
            "distribution_people_change": "2",
            "distribution_house_change": "3",
            "distribution_id": 1,
            "distribution_name": "主站TFF"
        }
    }
}
```

### translate old product ids to new, or new ids to old.
POST /control_stock/translateIds
```
params:
product_ids   # product ids,must be array(must param)
get_new_id   # the type is bool. If the value is 0 means old product ids to new,else new ids to old(must param)

Give an example with params
{
    "product_ids": [273106,273691],
    "get_new_id": 1
}

response:
{
    "code": 0,
    "message": "success",
    "data": {
        "273106": 101818154,
        "273691": 102202331
    }
}
```