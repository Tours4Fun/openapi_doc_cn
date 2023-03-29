# Create order

**Description**

V2 Version Create order API

### API URL

    POST	/v2/order/add

**Parameter**

| parameter           | type          | required | description             |
| -------------- |:-------------:| ----:| -----------------:|
| product_id    | integer  |  yes   | product id   |
| departure_date     | string  |  yes   |  departure date|
| departure_address  |string   |  yes   | departure address|
| upgrades           | array   |  yes   | upgrade（upgrade_id：upgrade_option_id）|
| rooms              | array   |  yes   | room info|
| --adult            | integer |  yes   | adult number |
| --kid              | integer |  yes   | kid number |
| --single_pairup    | integer |  no   | single pairup: yes no |
| contact     | array     |  yes   | contact|
| -first_name      | string     |  yes   | first name|
| -last_name       | string     |  yes   | last name|
| -mobile          |   string   |  yes   | mobile|
| -email           | string     |  yes   | email|
| guest_info  | array     |  yes   | guest info|

**Response**

| parameter           | type          | description             |
| -------------- |:-------------:|:-----------------:|
| code | integer|   0, -1 success, fail|
| msg  | string | success |
| data | array  |  array or empty array |
| -order_id | integer  |  order id |


**Reqeust parameter example**

```
{
    "product_id":102202692,
    "departure_date":"2019-01-16",
    "departure_address":"jhjhj",
    "upgrades":{
        "30100":["30577"]      //from product upgrades api upgradesid : [ option_id ]
    },
    //room info
    "rooms":[
        {
            "adult":2,
            "kid":0,
            "single_pairup":0
        }
    ],
    "contact":{
        "first_name":"a",
        "last_name":"b",
        "mobile":"1",
        "email":"2@q.q"
    },
    "guest_info":[
        //The following fields come from the PassengerForm obtained from the product API. After assembling each field, put it here, the following three fields are just examples, please refer to the fields returned by the specific product interface for details
        {
            "type":"adult",
            "firstname_en":"ghghg",
            "mobile":"86-6767"
        },
        {
            "type":"child",
            "firstname_en":"oooo",
            "mobile":"86-67887"
        }
    ]
}
```

**Response**

```
{
	"code": 0,
	"msg": "",
	"data": {
	   "order_id": 10004000
	}
}
```
