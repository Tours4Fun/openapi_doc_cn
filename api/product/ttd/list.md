# Product List

### Description

    Get the product list

### API address

    ttd/product/list

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
| product_region                    |     Product region chinese name[See Table.1 for all regions]                   |
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
                    "duration": 15,
                    "duration_type": "day",
                    "product_region": "佛州",
                    "product_sub_region": "",
                    "last_update": 1548180125
                }
            ]
        }
    }
    
    
Table 1.[Product region]

| region_name_en  | product_region | product_sub_region  |
| ------------- |:---------     | ---------------------|
| west         | 美国            | 美西               |
| east         | 美国            | 美东               |
| middle       | 美国            | 美中西             |
| florida      | 美国            | 佛州               |
| hawaii       | 美国            | 夏威夷             |
| alaska       | 美国            | 阿拉斯加           |
| south        | 美国            | 美南               |
| east         | 加拿大          | 加东               |
| west         | 加拿大          | 加西               |
|              | 拉美            | 墨西哥             |
|              | 拉美            | 其他拉美地区       |
| au           | 澳新            | 澳大利亚           |
| nz           | 澳新            | 新西兰             |
|              | 非洲            | 非洲               |
|              | 亚洲            | 亚洲其它           |
|              | 亚洲            | 中国               |
|              | 海岛目的地      | 海岛               |
|              | 海岛目的地      | 大洋洲             |
|              | 其他            | 其他               |
| north        | 欧洲            | 北欧               |
| middle       | 欧洲            | 中欧               |
| east         | 欧洲            | 东欧               |
| west         | 欧洲            | 西欧               |
| south        | 欧洲            | 南欧               |
| britain      | 欧洲            | 英国               |
| russia       | 欧洲            | 俄罗斯             |
| cuba         | 拉美            | 古巴               |
| ireland      | 欧洲            | 爱尔兰             |


