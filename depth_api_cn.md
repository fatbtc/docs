# 市场深度API

建议中国大陆用户使用www.fatbtc.us

API地址：

          https://www.fatbtc.com/m/depth/{symbol}
	  
          其中{symbol}表示交易对

          例如：
          https://www.fatbtc.com/m/depth/BTCFCNY

返回结果为JSON对象，形式如下：


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




关键返回值说明：

		symbol: 交易对
		timestamp: 时间戳
		bids: 买盘
		asks: 卖盘

		bids: [[价格，数量],[价格，数量],[价格，数量],...]
		asks: [[价格，数量],[价格，数量],[价格，数量],...]
