# 市场行情API


API地址：

          https://www.fatbtc.com/m/allticker/{timestamp}
          其中{timestamp}表示当前时间戳

          例如：
          https://www.fatbtc.com/m/allticker/1513327434000

返回结果为JSON对象，形式如下：

		{
			"state":1,
			"msg":"success",
			"data":{
				"wkcfcny_ticker":
				{
					"state":1,
					"msg":"success",
					"dspName":"WKC/FCNY",
					"symbol":"wkcfcny",
					"timestamp":1513327412135,
					"open":5.23,
					"high":5.299,
					"low":4.8,
					"close":4.99,
					"count":154,
					"volume":151744.8,
					"amount":63626.3828,
					"bis1":[4.95,37],
					"ask1": [5.09,92.4],
					"upOrDown":1,
					"pricePrecision":3,
					"volumePrecision":1,
					"order":1,
					"areaId":1,
					"canBuy":1,
					"canSell":1,
					"stopDesc":null
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

