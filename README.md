# Title: Trading Strategy Based on Fund Flow

## Summary: This strategy is based on a published paper, I extracted features from the paper and use mean-reverse model to make prediction. 

+ Tested Instrument: SP500 

+ Tested Period: 17 years data

+ Performance: For different strategy, we have different performance. The picture result is listed in the output folder. Data result is in Output data folder

### return like this

![Screenshot](https://github.com/ZishuoLi/Trading-Strategy-Based-On-Fund-Flow/blob/master/Output/12_ans.png)

![ScreenShot](https://github.com/ZishuoLi/Trading-Strategy-Based-On-Fund-Flow/blob/master/Output/17_ans.png)


![Link to performance ](https://github.com/ZishuoLi/Trading-Strategy-Based-On-Fund-Flow/tree/master/Output/1year_ans.png)


    12 days: based on Return/Volatility=4.5, Benchmark=2.95. (short term strategy)

    17 days: based on Return=518%, Benchmark=124%. (short term strategy)

    One year: Based on Return/Volatility, Return/Volatility=4.97, Benchmark=2.95 (long term strategy)


+ Impression: This project is done based on my interest, there could be huge improvement space. Due to other intern project and course burden, I don't have time to improve it, I will try to improve it later when I am free.


+ Overview


Reversion model based on Fund Flow. 
(If x days moving average of Fund Flow crossover above y days moving average, short SPY, otherwise long SPY

This model believe that strategy has continuation. In this model, strategy is updated every fixed period (Tested). Current strategy is selected from the optimal strategy of last period. Eg: last week, 7, 22 days moving average of Fund Flow works well, this week we continue use 7, 22 days moving average as strategy. 

I tested 3 to 40 days, month, season, half year, year as strategy update period and picked 12 days, 17 days & one year. 

Methodology

Investment Universe: SPY (SPDR S&P 500)

Trading Strategy: Long-short strategy. We short or long 100% ETF based on signal. 
	
Rebalancing Frequency: Strategy is updated every fixed period. Position is updated on daily level based on signals 
Backtested Performance

   Three period selected period: 12 days, 17 days, one year.

 
               




