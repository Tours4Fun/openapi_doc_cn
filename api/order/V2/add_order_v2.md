# 创建订单

**描述**

V2版本 创单接口

### API地址

    POST	/v2/order/add

**参数**

| 参数           | 类型          | 是否必须 | 描述             |
| -------------- |:-------------:| ----:| -----------------:|
| product_id    | integer  |  是   | 产品ID   |
| adult         | integer  |  是   | 成人数量 |
| kid           | integer |  是    | 小孩数量 |
| departure_date     | string  |  是   |  出团日期|
| departure_address  |string   |  是   | 出发地点|
| upgrades           | array   |  是   | 升级项（升级项ID：升级项子项ID）|
| rooms              | array   |  是   | （非票务产品参数）房间信息（含，成人数，儿童数，是否单人配方）|
| --adult            | integer |  是   | 成人数量 |
| --kid              | integer |  是   | 儿童数量 |
| --single_pairup    | integer |  否   | 是否单人配房 |
| tickets            | array   |  是   | （票务产品参数）房间信息（含，成人数，儿童数，是否单人配方）|
| --sku_id           | integer |  是   | sku id  |
| --count            | integer |  是   | 购买数量 |
| contact     | array     |  是   | 联系人信息|
| -first_name      | string     |  是   | 名|
| -last_name       | string     |  是   | 姓|
| -mobile          |   string   |  是   | 电话|
| -email           | string     |  是   | 邮箱|
| guest_info  | array     |  是   | 出行人信息（此参数根据产品获取的PassengerForm变化而不同）|

**返回**

| 参数           | 类型          | 描述             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 成功, 失败| 
| msg  | string | success |
| data | array  |  数组或空数组 |
| -order_id | integer  |  订单ID |


**请求参数示例**

（以下请求参数适用于一日游，多日游产品线）
```
{
    "product_id":102202692,  
    "adult":1,          
    "kid":1,            
    "departure_date":"2019-01-16",   //出团日期
    "departure_address":"jhjhj",     //出团地点
    "upgrades":{        
        "30100":["30577"]      //通过产品升级项接口获取到的 upgradesid : [ option_id ]
    },
    //房间信息
    "rooms":[       
        {
            "adult":2,             //成人人数
            "kid":0,               //儿童人数
            "single_pairup":0      //是否单人配房
        }
    ],
    //联系人信息
    "contact":{     
        "first_name":"a",
        "last_name":"b",
        "mobile":"1",
        "email":"2@q.q"
    },
    //出行人信息（可多个）
    "guest_info":[
        //以下的字段来自于从产品接口获取到的PassengerForm，对每个字段进行组装后，
        //放入这里，以下三个字段只是举例，详细请看具体产品接口返回的各个字段      
        {
            "type":"adult",
            "firstname_en":"ghghg",
            "mobile":"86-6767"
        },
        {
            "type":"kid",
            "firstname_en":"oooo",
            "mobile":"86-67887"
        }
    ]
}
```
（以下参数适用于票务产品线）
```
{
    "product_id":102202730,  
    "adult":1,          
    "kid":1,            
    "departure_date":"2019-01-16",   //出团日期
    "departure_address":"jhjhj",     //出团地点
    "upgrades":{       
        "219":["1375"],   //通过产品升级项接口获取到的 upgradesid : [ option_id ]
        "221":["1378"]
    },
    "tickets":[
        {
            "sku_id":15021,
            "count":1
        }
    ],
    //联系人信息
    "contact":{
        "first_name":"a",   
        "last_name":"b",
        "mobile":"1",
        "email":"2@q.q"
    },
    //出行人信息（可多个）（因票务产品无出行人信息，此项可不传）
    "guest_info":[
        {
            "type":"adult",         
            "firstname_en":"ghghg",
            "mobile":"86-6767"
        },
        {
            "type":"kid",
            "firstname_en":"oooo",
            "mobile":"86-67887"
        }
    ]
}
```

**返回示例**

```
{
	"code": 0,
	"msg": "",
	"data": {
	   "order_id": 10004000
	}
}
```
