对于回归模型
1. 优选观察F统计量的p值，这个p值是对整个模型进行对假设检验。
假设各个系数为0。如果p值较大，无法拒绝原假设，无法证明至少有一个自变量对因变量有显著性影响。
2. 观察调和R2，越大说明模型自变量对因变量可解释的部分越大，模型预测性越好。

回归诊断：
1. 自变量和因变量存在线性关系
2. 残差基本服从正态分布--QQ图
3. 残差方差满足同方差性，基本不变。
   1. Scale-Location，纵坐标为标准化残差的平方根，残差越大，点位置越高。分布越随机越好
4. 残差之间相互独立。
   1. Residual-Leverage。每个数据点对回归线的影响力，通过改图可以剔除异常值的点，可以改善回归效果。
   2. 异常值分类：离群点，杠杆点，强影响点

离差平方和的分解: 
1. SST 总平方和
2. SSR 回归平方和-均值到预测值-可解释的平方和
3. SSE 残差平方和-预测值到真值-不可解释的平方和

SST = SSR+SSE   
R2 = SSR/SST

模型F检验：比较MSR同MSE


参考：
> https://www.bilibili.com/video/av51815891?from=search&seid=9979237500261451613