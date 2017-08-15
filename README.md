# CalculateVelocityForBlasiusL2

计算Paraview导出数据中Y方向速度场数据与Blasius理论解相对比的L2误差的小程序。

2017年8月13日14:41:30
* 初始提交

2017年8月15日22:43:54
* 增加Test_auto.cpp，对原来的Test.cpp增加了循环计算，不过在循环计算的实现过程中每次进入新的循环前由于没有清空数据结构，结果导致计算结果与非循环计算的不一致，一度颠覆了原结果，带来不小的困扰，找bug找了半天，逐行调试才解决，好久没有coding了，确实生疏了。
```cpp
rangeBox_vector.clear();
```