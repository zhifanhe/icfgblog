# Simpoint

1. 把程序切成等长不交叠的片段，片段长度一般50M~200M，称为Interval。
2. 对所有的片段提取BBV(Basic Block Vector) 表征程序片段的相似度向量，再对这些向量做k-means聚类，便可以区分出k类的程序片段，并且每种类型包含的片段数目不同，可以计算出不同类型片段所占的比例，成为权重。
3. 找出各个聚类中心的程序片段作为checkpoint。


[关于SimPoint的一些碎碎念](https://zhuanlan.zhihu.com/p/380561873)
[Simpoint 在 GEM5 里加速仿真, 1 minute = N day(s)](https://zhuanlan.zhihu.com/p/453370789)