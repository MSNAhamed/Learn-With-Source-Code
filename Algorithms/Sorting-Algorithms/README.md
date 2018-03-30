# Sorting Algorithms



## The Bubble Sort


The **bubble sort** makes multiple passes through a list. 
It compares adjacent items and exchanges those that are out of order. 
Each pass through the list places the next largest value in its proper place. 
In essence, each item “bubbles” up to the location where it belongs.

![alt text](https://github.com/MSNAhamed/Learn-With-Source-Code/blob/master/Algorithms/Sorting-Algorithms/Bubble-sort.gif)
![alt text](https://github.com/MSNAhamed/Learn-With-Source-Code/blob/master/Algorithms/Sorting-Algorithms/BubbleSort_Avg_case.gif)

## The Selection Sort

The **selection sort** improves on the bubble sort by making only one exchange for every pass through the list.
 In order to do this, a selection sort looks for the largest value as it makes a pass and, after completing
 the pass, places it in the proper location. As with a bubble sort, after the first pass, the largest item is
 in the correct place. After the second pass, the next largest is in place. This process continues and requires 
 n−1n−1passes to sort _n_ items, since the final item must be in place after the (n−1)(n−1) st pass.

![alt text](https://github.com/MSNAhamed/Learn-With-Source-Code/blob/master/Algorithms/Sorting-Algorithms/Selection-Sort.gif)

## The Insertion Sort

We begin by assuming that a list with one item (position 0) is already sorted. On each pass, one for each item 1 
through n−1, the current item is checked against those in the already sorted sublist. As we look back into the 
already sorted sublist, we shift those items that are greater to the right. When we reach a smaller item or the 
end of the sublist, the current item can be inserted.

![alt text](https://github.com/MSNAhamed/Learn-With-Source-Code/blob/master/Algorithms/Sorting-Algorithms/Insertion-sort.gif)


