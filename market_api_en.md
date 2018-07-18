# Market Quotations API

API address：
          https://www.fatbtc.com/m/allticker/{timestamp}
         {timestamp} means current time stamp

For example：
          https://www.fatbtc.com/m/allticker/1513327434000
   

Return JSON Object as follows：

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
