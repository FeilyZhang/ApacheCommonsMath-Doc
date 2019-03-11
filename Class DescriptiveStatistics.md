# Class DescriptiveStatistics
## 变量
|变量名|描述|
|-----|-----|
|`static int INFINITE_WINDOW`|类变量，其创建一个不限制数据集大小的`DescriptiveStatistics`对象|
|`protected int	windowSize`|成员变量，可通过`setWindowSize(int windowSize)`方法重新设置数据集大小，然后再通过`addValue(double v)`方法追加数据，也可以通过`getWindowSize()`获取数据集大小，一般数据集的遍历会使用到|

## 构造器
|构造器|描述|
|-----|-----|
|`DescriptiveStatistics()`|无参构造器，需要通过`addValue(double v)`方法将数据逐一添加至数据集|
|`DescriptiveStatistics(DescriptiveStatistics original)`|传递一个`DescriptiveStatistics`型对象，描述性统计基于该对象的double型数组|
|`DescriptiveStatistics(double[] initialDoubleArray)`|传递一个形参为double型的数组，描述性统计均基于该数组|
|`DescriptiveStatistics(int window)`|int型参数window将会限制数据集中数据的个数，需要谨慎使用|

## 方法（常用）
|方法名|描述|
|-----|-----|
|`void addValue(double v)`|将数据v追加至数据集末尾|
|`DescriptiveStatistics copy()`|该方法返回当前`DescriptiveStatistics`类实例，可以直接获取相关统计量|
|`static void copy(DescriptiveStatistics source, DescriptiveStatistics dest)`|类方法，将source拷贝至dest|
|`double	getElement(int index)`|根据索引获取数据集中数据|
|`double	getGeometricMean()`|计算数据集的几何平均数|
|`double	getMax()`|获取数据集的最大值|
|`double	getMean()`|获取数据集的算数平均数|
|`double	getMin()`|获取数据集的最小值|
|`long getN()`|返回数据集中可用值得数目|
|`double getPercentile(double p`)|返回数据集的百分位数估计值|
|`double	getPopulationVariance()`|返回数据集的总体方差|
|`double[] getSortedValues()`|对数据集按照升序排序|
|`double	getStandardDeviation()`|返回数据及标准差|
|`double	getSum()`|对数据集求和|
|`double getSumsq()`|返回可用值的平方和|
|`double[]	getValues()`|返回当前数据集|
|`double	getVariance()`|返回可用数据集的样本方差|
|`int getWindowSize()`|获取数据集上限大小|
|`void removeMostRecentValue()`|从数据集中删除最近添加的值，即数据集的最后一个值|
|`double replaceMostRecentValue(double v)`|从数据集中替换最近添加的值为v|
|`void setWindowSize(int windowSize)`|设置数据集上限大小|
|`String	toString()`|生成数据集可用值的单变量统计信息报告|
