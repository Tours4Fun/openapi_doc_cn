# Product List

### Description

    Get the product list

### API address

    api_open/product/list

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| page                | int           |     No      |   Page page number[default:1]         |
| pageSize            | int           |     No      |   Number of paged data[default:20,max:50]          |
| lastUpdate          | int           |     No      |   Last update time, Unix timestamp[default:null]【The returned data will be greater than or equal to this value】           |

### Request parameter demo

	{
    	"page":1,
    	"pageSize":10,
    	"lastUpdate":1547748250
    }

### Request parameter description

| Field                             | Type          |     Description               |
| -------------------               |:-------------:|  :-----------------------     |
| product_id                        | int           |     Page page number[default:1]                      |
| name                              | int           |     Number of paged data[default:20,max:50]          |
| image_url                         | int           |     Number of paged data[default:20,max:50]          |
| product_line                      | int           |     Number of paged data[default:20,max:50]          |
| duration                          | int           |     Number of paged data[default:20,max:50]          |
| duration_type                     | int           |     Number of paged data[default:20,max:50]          |
| sub_region                        | int           |     Number of paged data[default:20,max:50]          |
| sub_region_chinese_name           | int           |     Number of paged data[default:20,max:50]          |
| region                            | int           |     Number of paged data[default:20,max:50]          |
| region_chinese_name               | int           |     Number of paged data[default:20,max:50]          |
| departure_city                    | int           |     Number of paged data[default:20,max:50]          |
| departure_city.id                 | int           |     Number of paged data[default:20,max:50]          |
| departure_city.name_en            | int           |     Number of paged data[default:20,max:50]          |
| departure_city.name               | int           |     Number of paged data[default:20,max:50]          |
| return_city                       | int           |     Number of paged data[default:20,max:50]          |
| return_city.id                    | int           |     Number of paged data[default:20,max:50]          |
| return_city.name_en               | int           |     Number of paged data[default:20,max:50]          |
| return_city.name                  | int           |     Number of paged data[default:20,max:50]          |
| visited_city                      | int           |     Number of paged data[default:20,max:50]          |
| visited_city.id                   | int           |     Number of paged data[default:20,max:50]          |
| visited_city.name_en              | int           |     Number of paged data[default:20,max:50]          |
| visited_city.name                 | int           |     Number of paged data[default:20,max:50]          |
| last_update                       | int           |     Number of paged data[default:20,max:50]          |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "count": 87,
            "page": 1,
            "page_size": 10,
            "products": [
                {
                    "product_id": 101461998,
                    "name": "(12天)哥伦比亚，厄瓜多尔，秘鲁三国休闲之旅",
                    "image_url": "//images/201510081444329046_5616b6565d06a_watermark_800_800.jpg",
                    "product_line": "ttd",
                    "duration": 12,
                    "duration_type": "day",
                    "sub_region": "",
                    "sub_region_chinese_name": "其他拉美地区",
                    "region": "latin-america",
                    "region_chinese_name": "拉美",
                    "departure_city": [
                        {
                            "id": 717,
                            "name_en": "Bogota",
                            "name": "波哥大"
                        }
                    ],
                    "return_city": [
                        {
                            "id": 1010,
                            "name_en": "Cusco",
                            "name": "库斯科"
                        }
                    ],
                    "visited_city": [
                        {
                            "id": 669,
                            "name_en": "Quito",
                            "name": "基多"
                        },
                        {
                            "id": 671,
                            "name_en": "Lima",
                            "name": "利马"
                        },
                        {
                            "id": 717,
                            "name_en": "Bogota",
                            "name": "波哥大"
                        },
                        {
                            "id": 719,
                            "name_en": "Cartagena",
                            "name": "卡塔赫纳"
                        },
                        {
                            "id": 1010,
                            "name_en": "Cusco",
                            "name": "库斯科"
                        }
                    ],
                    "last_update": 1547748250
                }
                ......
            ]
        }
    }


