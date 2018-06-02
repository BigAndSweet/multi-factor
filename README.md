# alpha
从数据库提取数据构建因子，测试因子的有效性，包括因子收益率、因子收益率T值、IC值，分层测试以观察因子收益率的按照因子大小排序分组的不同组合的组合收益率、波动率、收益率的单调性、最大回测、夏普比率、信息比率等。
## self_libs , 自定义的一些模块

  1.data_clean.py，数据清洗  
  * 剔除存在ST标记的数据和上市不满一年的股票
  * MAD法去除异常值，Z-值标准化，然后对行业哑变量和对数值回归取残差，得到行业与市值中性化的因子值
  
  2.factor_test.py, 单因子有效性的评价指标
  * 因子收益率（均值、标准差)  
  $$R_{it} = \beta_{it} + \beta_{it} * f_{it}$$
  * 因子收益率的T值  
  * IC值
  
  3.class_test.py, 大类因子之间有效的比较  
  * 累计收益率
  * 单调性
  * IC值相关性

<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$\\(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}\\
<img src="http://chart.googleapis.com/chart?cht=tx&chl=\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" style="border:none;">
