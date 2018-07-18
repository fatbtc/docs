# Latest transaction API

Recommended for users in mainland China access www.fatbtc.us

API URL：

          https://www.fatbtc.com/m/trade/{symbol}/{size}/{ts}
	  
          {symbol}: trading pair
          {size}: number of data, value 1、10 value 1、10
          {ts}: timestamp

          For example：
          https://www.fatbtc.com/m/trade/BTCFCNY/10/1531836414856


The result is a JSON object, formats are as follow：

		{
		    "status": 1, 
		    "msg": "success", 
		    "symbol": "btcfcny", 
		    "timestamp": 1531836415123, 
		    "trades": [
			{
			    "id": null, 
			    "timestamp": 1531901229982, 
			    "volume": 0.6633, 
			    "price": 47577.59, 
			    "taker": "sell", 
			    "upOrDown": -1
			}, 
			...
		    ]
		}


Key reture value description：

		id: ID
		price: Executed price
		taker: taker (buy: buy, sell: sell) 
		timestamp: timestamp
		upOrDown: relative to the latest rise and fall in prices, 1 is up, -1 is down
		volume: executed amount 

