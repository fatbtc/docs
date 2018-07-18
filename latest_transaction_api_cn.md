
# 最新成交API

建议中国大陆用户使用www.fatbtc.us

API地址：

          https://www.fatbtc.com/m/trade/{symbol}/{size}/{ts}
	  
          {symbol}: 交易对
          {size}: 数据条数, 取值1、10
          {ts}: 时间戳

          例如：
          https://www.fatbtc.com/m/trade/BTCFCNY/10/1531836414856

返回结果为JSON对象，形式如下：

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


关键返回值说明：


		id: ID
		price: 成交价
		taker: 吃单方  (buy: 买入, sell: 卖出)
		timestamp: 时间戳
		upOrDown: 相对于最近一次价格的涨跌, 1涨, -1跌
		volume: 成交数量


