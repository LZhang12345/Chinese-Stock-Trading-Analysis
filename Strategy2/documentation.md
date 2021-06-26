We start by web scraping the table from url: http://fund.eastmoney.com/data/fundranking.html#tall;c0;r;sqjzf;pn50;ddesc;qsd20150101;qed20151231;qdii;zq;gg;gzbd;gzfs;bbzt;sfbb <br>
Unlike the normal procedures, this html contains "dynamic" contents. Therefore, we need to do more than directly scraping. <br>
<br>
Using the webdriver, we first use "self-defined" date range(xxxx-xx-xx -- xxxx-xx-xx) to search for the first 50 funds('混合型'). <br>
&emsp; It is noted that the first 50 funds will be enough, we've found out that  20, 25, 30, 35 will generate similar results. There's no need to 
&emsp; include more funds into the stats<br>
Then we 
