# 市场行情API

建议中国大陆用户使用www.fatbtc.us

API地址：

          https://www.fatbtc.com/m/allticker/1/{timestamp}
          其中{timestamp}表示当前时间戳

          例如：
          https://www.fatbtc.com/m/allticker/1/1513327434000

返回结果为JSON对象，形式如下：

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



关键返回值说明：

		dspName：交易对，以/分割，前面为基础货币，后面为计价货币
		open：24小时开盘价
		high：24小时最高价
		low：24小时最低价
		close：当前价格
		volume：24小时成交量
		bis1：买一价格，买一数量
		ask1：卖一价格，卖一数量
		upOrDown：相比较上一笔交易的涨跌
		canBuy: 是否可买入，1表示可买
		canSell: 是否可卖，1表示可卖
		pricePrecision: 价格小数位
		volumePrecision: 数量小数位
		minBuyVolume: 最小买入量
		minBuyAmount: 最小买入金额
		minSellVolume: 最小卖出量
		fixedBuyPrice: 固定买入价
		weekOpen: 7天内开盘价

