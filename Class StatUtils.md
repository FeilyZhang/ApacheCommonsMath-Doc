# Class StatUtils
该类是一个静态类，不需要构造器
## 方法（常用）
方法意义浅显易懂，只罗列不解释

|方法名|描述|
|-----|-----|
|`StatUtils.max(double[] values)`|...|
|`StatUtils.min(double[] values)`|...|
|`StatUtils.mean(double[] values)`|...|
|`StatUtils.percentile(double[] values)`|...|
|`StatUtils.sum(double[] values)`|...|
|`StatUtils.sumSq(double[] values)`|...|
|`StatUtils.populationVariance(double[] values)`|...|
|`StatUtils.variance(double[] values)`|...|

该类几乎所有的方法都会提供这样的参数列表, `(double[] values, int begin, int length)`, 表示计算数据集中指定范围的相关统计量。

## demo
[ApacheCommonsMath-Code StatUtilsDemo](https://github.com/FeilyZhang/ApacheCommonsMath-Code/blob/master/src/tech/feily/dataanalysis/demo/StatUtilsDemo.java)