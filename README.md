# tf-on-BTC
用tensorflow做BTC量化交易

# 大致思路

取连续360天作为训练集, 每天取前30天日均价格作为输入(360x30), 每天取次日价格为标准答案y, 训练一个RNN, 使L(y-RNN(x))最小.

# 安装

1. 下载python 3.6.latest
2. 安装依赖 `pip install -r requirments.txt`
3. 启动交互环境: `jupyter notebook`

# 参考

[六维数据](http://6vdata.com)是使用了类似思路做的A股预测(仅预测, 没有交易部分).