# Product list

### Description

Get a list of products based on `region`, `product line`, etc.


### API url

    /v2/product/list

### Parameter

| Parameter           | type          | required | description            |
| -------------- |:-------------:| ----:| :-----------------|
| region     | string  |  no   | product region  |
| product_line     | string  |  no   | ttd or tour  |
| page   | int  |  no   | default 1  |
| page_size   | int  |  no   | number of products per page, default 20  |
| keyword   | string  |  no   | keyword, such as product name  |

Note: `region`,`product_line`,`keyword` Pass at least one of these three parameters

region map:
us,ca,latin-america,europe,anz,cruise,africa,asia,island,other,west,east,middle,florida,hawaii,alaska,south,east,west,mexico,other,europe,au,nz,caribbean,mexico,alaska,hawaii,bermuda,europe,nordic,canada-coast-new-england,asia,polar,global,australia-new-zealand,other,other,china,island,oceania,other,north,middle,east,west,south,britain,russia,cuba,ireland,Japan-and-South-Korea-Cruise,Southeast-Asia-Cruise,Africa-Cruise,Middle-East-Cruise,South-America-Cruise,Panama-Cruise,US-and-Canada-Cruise,Pacific-Cruise,European-River-Cruise,Africa-River-Cruise,Asia-River-Cruise,North-America-River-Cruise,Russian-River-Cruise,South-America-River-Cruise,Costa-Rica,Peru,Ecuador,Brazil,seattle,Puerto Rico,The-United-Arab-Emirates,Japan,Qatar,Republic of Korea,Egypt,The-Kingdom-of-Morocco,Yellow-Stone

### Request parameter example

    {
    	"product_line" : "tour"
    }


### Response

	{
        "code": 0,
        "msg": "success",
        "data": {
            //total product number
            "count": "8851",
            //current page
            "page": "1",
            //number of products per page
            "page_size": "20",
            "products": [
                {
                    //product id
                    "product_id": "13374",
                    //product old id
                    "product_id_old": "103",
                    //product name
                    "name": "Los Angeles Disneyland Day Trip",
                    //product image
                    "image_url": "https://tffimg.tff.bz/c2/b0/c73/626/843f4f193a898543855e36.jpg",
                    //product line
                    "product_line": "tour",
                    //product duration
                    "duration": "3.0",
                    //product duration type: day,hour,minite
                    "duration_type": "day",
                    //product sub region
                    "sub_region": "west",
                    //product sub region chinese name
                    "sub_region_chinese_name": "美西",
                    //product region
                    "region": "us",
                    //product region chinese name
                    "region_chinese_name": "美国",
                    //advertised price
                    "advertised_price": "20.700001",
                    //product departure city
                    "departure_city": [
                        {
                            "id": 1,
                            "name_en": "Los Angeles",
                            "name": "洛杉矶"
                        }
                    ],
                    //product end city
                    "return_city": [
                        {
                            "id": 1,
                            "name_en": "Los Angeles",
                            "name": "洛杉矶"
                        }
                    ],
                    //product vistied city
                    "visited_city": [
                        {
                            "id": 1,
                            "name_en": "Los Angeles",
                            "name": "洛杉矶"
                        }
                    ]
                },
                {
                    "product_id": "13527",
                    "product_id_old": "240",
                    "name": "Big Island One Day Tour",
                    "image_url": "https://tffimg.tff.bz/e1/04/424/beb/abf7e56a478c2fb7e9c1d8.jpg",
                    "product_line": "tour",
                    "duration": "11.5",
                    "duration_type": "hour",
                    "sub_region": "hawaii",
                    "sub_region_chinese_name": "夏威夷",
                    "region": "us",
                    "region_chinese_name": "美国",
                    "advertised_price": "310.000000",
                    "departure_city": [
                        {
                            "id": 162,
                            "name_en": "Honolulu",
                            "name": "檀香山"
                        }
                    ],
                    "return_city": [
                        {
                            "id": 162,
                            "name_en": "Honolulu",
                            "name": "檀香山"
                        }
                    ],
                    "visited_city": [
                        {
                            "id": 162,
                            "name_en": "Honolulu",
                            "name": "檀香山"
                        }
                    ]
                }
            ]
        }
    }


