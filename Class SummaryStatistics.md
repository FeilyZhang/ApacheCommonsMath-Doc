# Class SummaryStatistics
## 构造器
|构造器|描述|
|-----|-----|
|`SummaryStatistics()`|无参构造器，通过`addValue(double value)`方法添加值|
|`SummaryStatistics(SummaryStatistics original)`|该构造器接收一个SummaryStatistics型对象，并在其基础之上运算|

## 方法（常用）
以下某些方法的使用和`DescriptiveStatistics`相似，不再解释

|方法名|描述|
|-----|-----|
|`void addValue(double value)`| ... |
|`SummaryStatistics	copy()`|...|
|`static void copy(SummaryStatistics source, SummaryStatistics dest)`|...|
|`double getGeometricMean()`|...|
|`double getMax()`|...|
|`double getMean()`|...|
|`double getMin()`|...|
|`long getN()`|...|
|`double getPopulationVariance()`|...|
|`double getStandardDeviation()`|...|
|`double getSum()`|...|
|`StatisticalSummary getSummary()`|返回当前统计信息的StatisticalsSummaryValues实例|
|`double getSumsq()`|...|
|`double getVariance()`|...|
|`int hashCode()`|基于统计值返回其哈希值|
|`String toString()`|...|
