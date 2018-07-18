# Depth API

Recommended for users in mainland China access www.fatbtc.us

API address：

          https://www.fatbtc.com/m/depth/{symbol}
	  
           {symbol} indicates the trading pair
        

          For example：
          https://www.fatbtc.com/m/depth/BTCFCNY

The result is a JSON object, formats are as follow：




		{
		    "status": 1, 
		    "msg": "success", 
		    "symbol": "btcfcny", 
		    "timestamp": 1531897561678, 
		    "bids": [
			[
			    46501.01, 
			    0.1669
			], 
			[
			    46501, 
			    0.22
			], 
			[
			    46000.1, 
			    0.036
			], 
			...
		    ], 
		    "asks": [
			[
			    48500, 
			    0.0139
			], 
			[
			    48555, 
			    0.0074
			], 
			[
			    49950, 
			    0.0979
			], 
			...
		    ]
		}




Key reture value description：

		symbol:  trading pair
		timestamp:  timestamp
		bids: bids
		asks: asks

		bids:  [[price,amount],[price,amount],[price,amount],...]
		asks:  [[price,amount],[price,amount],[price,amount],...]
