# ![](https://drive.google.com/uc?id=10INx5_pkhMcYRdx_OO4rXNXxcsvPtBYq) Quick Sort 快速排序
> ##### 理論請自行找，網路上有很多相關的文章，這邊只關注於範例實作的部分.

---

## 簡介
快速排序（Quick Sort）是一種高效的排序算法，它基於分治法(Divide and Conquer)的概念。<br>
該算法的基本思想是選擇一個基準元素（pivot），將數列分為比基準元素小的部分和比基準元素大的部分，<br>
然後對這兩部分進行遞迴排序。最終，所有的子部分排序完成後，整個數列就會有序。<br>
<br>
快速排序有多種實現版本，其中最常見的包括以下幾種：
- [Lomuto partition scheme（洛穆托分區方案）](https://github.com/RC-Dev-Tech/algorithm-quick-sort-lomuto): 這是快速排序算法中較簡單的一種實現方式。<br>
  它使用最右邊的元素作為基準點（pivot），將數列分成小於等於基準點和大於基準點的兩部分，並將基準點放在適當的位置。<br>
  這種實現方式在遇到大量重複元素時性能較差。
  
<br>

- [Hoare partition scheme（霍爾分區方案）](https://github.com/RC-Dev-Tech/algorithm-quick-sort-hoare): 這是快速排序算法中較為高效的一種實現方式。<br>
  它使用兩個指針，一個從數列左邊開始移動，一個從數列右邊開始移動，直到找到需要交換的元素，然後將它們交換。<br>
  這種實現方式在處理大量重複元素時性能較好。

<br>

- [內省式快速排序（Introsort）](https://github.com/RC-Dev-Tech/algorithm-quick-sort-introsort)：結合了快速排序和堆排序的優點，當分區的大小小於一個閾值時，轉而使用堆排序以避免快速排序的最差情況。

<br>

- [三路快速排序（Three-Way Quick Sort）](https://github.com/RC-Dev-Tech/algorithm-quick-sort-three-way) ：針對存在大量重複元素的情況進行優化，將數列分成小於、等於和大於基準點的三部分。

<br>

- [隨機化快速排序（Randomized Quick Sort）](https://github.com/RC-Dev-Tech/algorithm-quick-sort-randomized)：在選擇基準點時隨機選取，以減少對特定輸入的敏感性，提高性能的一種方法。

<br>

- [雙輪排序（Dual-Pivot Quick Sort）](https://github.com/RC-Dev-Tech/algorithm-quick-sort-dual-pivot)：使用兩個基準點將數列分成三部分，進一步減少排序過程中的比較和交換操作。

<br>

這些實現方式都是基於快速排序算法的基本思想，但在細節上有所差異，以適應不同的數據情況並提高性能。<br>
根據具體情況，選擇適合的實現方式可以提供更高效的排序結果。

