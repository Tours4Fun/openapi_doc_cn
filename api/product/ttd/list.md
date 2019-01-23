# Product List

### Description

    Get the product list

### API address

    api_open/product/list

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| page                | int           |     No      |   Page page number[default:1]         |
| page_size            | int           |     No      |   Number of paged data[default:20,max:50]          |
| last_update          | int           |     No      |   Last update time, Unix timestamp[default:null]【The returned data will be greater than or equal to this value】           |

### Request parameter demo

	{
    	"page":1,
    	"page_size":10,
    	"last_update":1547748250
    }

### Return field description

| Field                             |     Description                                   |
| -------------------               |  :-----------------------                         |
| product_id                        |     Product unique id                             |
| name                              |     Product name                                  |
| image_url                         |     Product image url                             |
| duration                          |     Product duration                              |
| duration_type                     |     Product duration unit[min,hour,day]           |
| product_region                    |     Product region chinese name                   |
| product_sub_region                |     Product sub region chinese name               |
| last_update                       |     Product last update time                      |


### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "count": 12476,
            "page": 1,
            "page_size": 2,
            "products": [
                {
                    "product_id": 20112,
                    "name": "8-Day A Taste Of San Francisco & Napa Valley Bus Tour",
                    "image_url": "http://toursforfun.tff.bz/images/new-orleans_2.jpg",
                    "product_line": "tour",
                    "duration": 12,
                    "duration_type": "day",
                    "product_region": "",
                    "product_sub_region": "",
                    "last_update": 1548180123
                },
                {
                    "product_id": 20157,
                    "name": "Totem Circle  With Vancouver Extension",
                    "image_url": "http://toursforfun.tff.bz/images/201406061402033941_5391571503817_watermark_800_800.jpg",
                    "product_line": "tour",
                    "duration": 15,
                    "duration_type": "day",
                    "product_region": "佛州",
                    "product_sub_region": "",
                    "last_update": 1548180125
                }
            ]
        }
    }


