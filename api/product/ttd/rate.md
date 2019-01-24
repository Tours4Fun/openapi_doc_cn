# Currency exchange rate

### Description

    Get currency exchange rate

### API address

    ttd/rate

### Request parameter description

| Parameter           | Type          | Is required | Description             |
| ------------------- |:-------------:| -----------:| :-----------------------|
| date          | date         |     No     |   eg:2019-01-23 18:18:00        |


### Request parameter demo

	{
    	"date":"2018-02-02 12:12:12"
    }

### Return field description

    
### Interface return

	{
        "code": 0,
        "msg": "success",
        "data": {
            "USD": 1,
            "GBP": 0.7,
            "AUD": 1.2441,
            "NZD": 1.3564,
            "EUR": 0.8027,
            "CAD": 1.2282,
            "SUR": 56.0871,
            "JPY": 109.3553,
            "ZAR": 11.8628,
            "NOK": 7.6715,
            "PHP": 51.4666,
            "SEK": 7.8597,
            "CHF": 0.9301,
            "DKK": 5.9746,
            "HKD": 7.8237,
            "THB": 31.2831,
            "CNY": 6.3098,
            "RUB": 56.0871
        }
    }



