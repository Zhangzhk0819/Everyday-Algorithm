## 5.5 快速排序
### 核心思想
1. 快速排序算法的计算复杂度非常低，只有O(nlgn)，其思想也非常巧妙，所以很值得学习。
2. 快排的核心思想是分治，首先选取一个参考值a，如果作升序排序，那么把比a小的值放在a左边，把比a大的值放在a右边，然后对a左边和右边序列再分别做快排，直到所有元素按升序排列。

### [程序实现](https://github.com/Zhangzhk0819/Everyday-Algorithm/blob/master/Code/Quicksort.cpp)
1. 整个程序框架使用递归算法。
2. 在每一步快排过程中，使用两个指针，分别指向数组首部和尾部，并把第一个元素作为参考值a，首先通过移动尾部指针，找到小于a的值，与a交换位置，然后通过移动首部指针，找到大于a的值，与a交换顺序，最后依次移动首尾指针，直到两个指针相遇，就完成了单步快排。

### 示例
假设数组 6 2 7 3 8 9  
1. 6 2 7 3 8 9  
2. 3 2 7 6 8 9  
3. 3 2 6 7 8 9  
4. 2 3 6 7 8 9

Reference:[百度百科](http://baike.baidu.com/link?url=QzOZlOqZFiPO82cpEOFH143ewPZdH7N1fS5ucXhjuYPL5Bxtan2ooV0gkPl9Dic2Lc3ggD6gjGA0sw1CsckQ2-TD9woGOxLozRGGGb3zLiJuN84xciMtAttZG-74C18_aXYiX_O0DT15XE_xzbdoOfK7VqvtMSObSiXX2O6oJIe2Z4Lv0JbiLbI5wejRGp_a)

