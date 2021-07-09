## Chinese-Stock-Trading-Analysis

1. 分析每季度各个基金排行情况 <br>
股票型：<br>
https://fund.eastmoney.com/data/fundranking.html#tgp;c0;r;s1nzf;pn50;ddesc;qsd20200103;qed20210103;qdii;zq;gg;gzbd;gzfs;bbzt;sfbb <br>
混合型：<br>
https://fund.eastmoney.com/data/fundranking.html#thh;c0;r;s1nzf;pn50;ddesc;qsd20200103;qed20210103;qdii;zq;gg;gzbd;gzfs;bbzt;sfbb <br>
前50排名
目前，我们可以 <br>
1）根据每三个月的一次基金排名公布来调整仓位，但是这样会有很大的滞后 <br>
&emsp; 首先我们根据2020四个季度的数据来改变下个季度的仓位，详细数据和文档放在Strategy1里面 <br>
&emsp; ![alt text](https://github.com/LZhang12345/Chinese-Stock-Trading-Analysis/blob/main/Strategy1/Strategy%201-%203%20month%20period%2C%2020200407--20210407.png) <br>
&emsp; 我们可以看到，从2020/04/07到2021/04/07，我们的收益率是80%+ <br>
&emsp; 这样做的弊端就在于调整时间过于冗长，从而导致很难捕捉到确切的信号。举个例子，假设4/7公布截止3/31的持仓数据，那么从4/7到7/7我们都只能依靠3/31的数据，当时间越往后,这个信息的可靠性就越低。<br>
2）很明显我们不可能获取及时的基金仓位变化情况，但是我们可以根据尽最大可能提升这个数据的可靠性。比如我们可以再某个时间段内对基金收益率进行排名，然后这些获取最近一个季度的持仓情况。<br>
&emsp; 我们测试了各种策略，就目前来说收益率最好的策略是，获取当前4周的基金排名以及仓位情况，选出10支来进行未来2周/1周的持仓策略 <br>
&emsp; 4周/2周 2021/04/07 -- 2021/06/18<br>
&emsp; ![alt text](https://github.com/LZhang12345/Chinese-Stock-Trading-Analysis/blob/main/Strategy2/4weeks:2weeks.png) <br>
&emsp; 4周/1周 2021/04/07 -- 2021/06/25<br>
&emsp; ![alt text](https://github.com/LZhang12345/Chinese-Stock-Trading-Analysis/blob/main/Strategy2/4weeks:1week.png) <br>
&emsp; 我们可以看到，2周表现得更好且更稳定。我们可以发现，这种策略没有办法回避回调带来的影响，但是可以最大程度地在指数上扬的时候增加收益 <br>

根据估算，收益率大致与当年第50位左右的基金持平。罗列出近十年来所有基金的收益情况，统计如下：
2020	1	2
2019	0.8	1.8
2018	0.05	1.05
2017	0.4	1.4
2016	0.14	1.14
2015	0.81	1.81
2014	0.48	1.48
2013	0.36	1.36
2012	0.15	1.15
2011	-0.1	0.9
		22.7480532![image](https://user-images.githubusercontent.com/51413837/125009706-af589b00-e02a-11eb-8ac0-60fe87584c45.png)


2. 根据分析结果，选择持仓比例

3. 比较与上一季度的持仓情况，选择性调整

4. 仓位和资金动向追踪
