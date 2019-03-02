# Market Quotations API

API address：
          https://www.fatbtc.com/m/allticker/1/{timestamp}
         {timestamp} means current time stamp

For example：
          https://www.fatbtc.com/m/allticker/1/1513327434000
   

Return JSON Object as follows：

          {
                    "state":1,
                    "msg":"success",
                    "data":{
                              "wkcfcny_ticker":
                              {
                                        "status": 1,
				      "msg": "success",
				      "dspName": "WKC/FCNY",
				      "symbol": "wkcfcny",
				      "timestamp": 1551495353625,
				      "open": 0.3712,
				      "high": 0.3762,
				      "low": 0.3527,
				      "close": 0.3554,
				      "count": 469,
				      "volume": 1029806.54,
				      "amount": 371036.701985,
				      "bis1": [0.3501, 172.69],
				      "ask1": [0.36, 639.19],
				      "upOrDown": -1,
				      "pricePrecision": 4,
				      "volumePrecision": 2,
				      "order": 230,
				      "areaId": 4,
				      "canBuy": 1,
				      "canSell": 1,
				      "stopDesc": "",
				      "quoteCurrencyName": "",
				      "baseCurrencyName": "WKC",
				      "minBuyVolume": 5,
				      "minBuyAmount": 0,
				      "minSellVolume": 5,
				      "fixedBuyPrice": 0,
				      "weekOpen": 0.3188,
				      "siteId": 1
                              },
                              ......
                    }
          }


Explanation of key points：

		dspName：the trade pairs, WKC/FCNY means WKC is the basic money and FCNY is the account money;
		open：the open price, for a 365x24 running market, it’s the price of 24 hours ago
		high：the highest price of last 24 hours
		low：the lowest price of last 24 hours
		close：the last transaction price
		volume：the volumes of last 24 hours
		bis1：the bid1 price and amount
		ask1：the ask1 price and amount
		upOrDown：compare with the last transaction, the range of rise and fall of current transaction price
		canBuy: Can I buy, 1 is you can buy
		canSell: Can I sell, 1  is you can buy
		pricePrecision: price decimal place
		volumePrecision: number of decimal places
		minBuyVolume: minimum purchase amount
		minBuyAmount: minimum purchase amount
		minSellVolume: minimum sell volume
		fixedBuyPrice: fixed buy price
		weekOpen: opening price within 7 days
	  
