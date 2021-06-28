## Chinese-Stock-Trading-Analysis

1. 分析每季度各个基金排行情况 <br>
股票型：<br>
https://fund.eastmoney.com/data/fundranking.html#tgp;c0;r;s1nzf;pn50;ddesc;qsd20200103;qed20210103;qdii;zq;gg;gzbd;gzfs;bbzt;sfbb <br>
混合型：<br>
https://fund.eastmoney.com/data/fundranking.html#thh;c0;r;s1nzf;pn50;ddesc;qsd20200103;qed20210103;qdii;zq;gg;gzbd;gzfs;bbzt;sfbb <br>
前50排名
目前，我们可以 <br>
&emsp; 1）根据每三个月的一次基金排名公布来调整仓位，但是这样会有很大的滞后 <br>
&emsp; 首先我们根据2020四个季度的数据来改变下个季度的仓位，详细数据和文档放在Strategy1里面 <br>
&emsp; ![alt text](https://github.com/LZhang12345/Chinese-Stock-Trading-Analysis/blob/main/Strategy1/Strategy%201-%203%20month%20period%2C%2020200407--20210407.png) <br>
&emsp; 我们可以看到，从2020/04/07到2021/04/07，我们的收益率是80%+ <br>
&emsp; 这样做的弊端就在于调整时间过于冗长，从而导致很难捕捉到确切的信号。举个例子，假设4/7公布截止3/31的持仓数据，那么从4/7到7/7我们都只能依靠3/31的数据，当时间越往后，
&emsp; 这个信息的可靠性就越低。<br>
&emsp; 2）很明显我们不可能获取及时的基金仓位变化情况，但是我们可以根据尽最大可能提升这个数据的可靠性。比如我们可以再某个时间段内对基金收益率进行排名，然后这些获取最近一个季度的持仓情况。<br>
&emsp; 我们测试了各种策略，就目前来说收益率最好的策略是，获取当前4周的基金排名以及仓位情况，选出10支来进行未来2周/1周的持仓策略 <br>
&emsp;

2. 根据分析结果，选择持仓比例

3. 比较与上一季度的持仓情况，选择性调整

4. 仓位和资金动向追踪
