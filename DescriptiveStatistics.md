# Class DescriptiveStatistics
## 变量
|变量名|描述|
|-----|-----|
|`static int	INFINITE_WINDOW`|类变量，其创建一个不限制数据集大小的`DescriptiveStatistics`对象|
|`protected int	windowSize`|成员变量，可通过`setWindowSize(int windowSize)`方法重新设置数据集大小，也可以通过`getWindowSize()`获取数据集大小，一般数据集的遍历会使用到|

## 构造器
|构造器|描述|
|-----|-----|
|`DescriptiveStatistics()`|无参构造器，需要通过`addValue(double v)`方法将数据逐一添加至数据集|
|`DescriptiveStatistics(DescriptiveStatistics original)`|传递一个`DescriptiveStatistics`型对象，描述性统计基于该对象的double型数组|
|`DescriptiveStatistics(double[] initialDoubleArray)`|传递一个形参为double型的数组，描述性统计均基于该数组|
|`DescriptiveStatistics(int window)`|int型参数window将会限制数据集中数据的个数，需要谨慎使用|

## 