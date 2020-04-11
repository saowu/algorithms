# algorithms
>《algorithms》学习笔记

[![Build Status](https://img.shields.io/travis/otale/tale.svg?style=flat-square)](https://github.com/saowu/algorithms)
[![License](https://img.shields.io/badge/license-MIT-4EB1BA.svg?style=flat-square)](https://github.com/saowu/algorithms)
[![GitHub forks](https://img.shields.io/github/forks/saowu/algorithms.svg?style=flat-square)](https://github.com/saowu/algorithms/network)
[![GitHub stars](https://img.shields.io/github/stars/saowu/algorithms.svg?style=flat-square)](https://github.com/saowu/algorithms/stargazers)

[下载 algs4.jar](https://algs4.cs.princeton.edu/code/algs4.jar)

### 一、排序
#### 1.初级排序算法
##### 1.1选择排序

>命题：对于长度为N的数组，选择排序算法需要大约`N^2`次比较和`N`次交换。

算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
选择排序 | `O(n^2)` | `O(n^2)` | ` O(1) ` | 否
##### 1.2插入排序
>命题：对于随机排列的长度为` N `且主键不重复的数组，平均情况下插入排序需要` ~N^2/4 `次比较以及` ~N^2/4 `次交换。最坏情况下需要` ~N^2/2 `比较和` ~N^2/2 `交换，最好情况下需要` N-1 `次和0次比较。

算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
插入排序 | ` O(n^2) ` | ` O(n^2) ` | ` O(1) ` | 是

##### 1.3希尔排序
>命题：使用递增序列1，4，13，40，121，364···的希尔排序所需的比较次数不会超过` N `的若干倍乘以递增序列的长度。

算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
希尔排序 | ` O(nlogn) ` | ` O(n^s) ` | ` O(1) ` | 否

#### 2.归并排序算法
##### 2.1自顶向下归并排序
>命题：对于长度为` N `的任意数组，自顶向下归并排序需要` 1/2NlgN `至` NlgN `次比较。

算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
自顶向下归并排序 | ` O(nlogn) ` | ` O(nlogn) ` | ` O(n) ` | 是


##### 2.1自底向上归并排序
>命题：对于长度为` N `的任意数组，自底向上归并排序需要` 1/2NlgN `至` NlgN `次比较，最多访问数组` 6NlgN `次。

算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
自底向上归并排序 | ` O(nlogn) ` | ` O(nlogn) ` | ` O(n) ` | 是


#### 3.快速排序算法
##### 3.1基本快速排序
>命题A：对于长度为` N `的无重复数组，快速排序算法平均需要`～2NlgN `次比较（以及1/6次的交换）。

>命题B：快速排序最多需要约`N^2/2`次比较，但随机打乱数组能够预防这种状况。

算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
基本快速排序 | ` O(nlogn)` | ` O(n^2） ` | ` O(logn) ` | 否

##### 3.2三向切分的快速排序
>命题：对于长度为` N `的数组，三向切分的快速排序算法平均需要`～（2lg2）NH `次比较。其中H为由主键值出现频率定义的香农信息量。


算法 | 平均时间复杂度 | 最坏时间复杂度 | 空间复杂度 | 是否稳定
---|---|---|---|---|
2三向切分的快速排序 | ` O(n)` | ` O(nlogn) ` | ` O(logn) ` | 否
