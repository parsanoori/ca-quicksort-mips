## Quicksort implementation in MIPS

Implement Quicksort algorithm in the `quicksort.asm` file.  
Quicksort is classified as a Divide and Conquer algorithm. The basic idea behind it is that when an element is known to be at its correct place, and all the elements before it are smaller than it and all the elements after it are bigger, we can safely sort the subarrys left and right of that element to sort the whole array.  
Hence first it's needed to place an element, namely pivot, at its right place. For that purpose in your implementation you have to choose a random element of the array and partition the array according to that pivot. After that, you have to sort the left and right subarrays.
For more information about Quicksort you can visit [this link](https://brilliant.org/wiki/quick-sort/#choosing-a-pivot).  
The `cppimpl` folder has the implementation of the algorithm in C++. You may want to take a look at it.  
The `mergesort.asm` has the implementation of the mergesort algorithm in MIPS assembly. You may want to take look it too.  

***Attention***: Implementing another method for choosing pivot leads to score loss.  

## Function

It simply sort an array.


### Input

In the first line, the count of the numbers to sort, n, is given.   
In the next n lines the elements of the array are given.


### Output

In each line of the output print each element of the ascending sorted array.

### Input Example 1

```
5
1
5
3
4
2
```

### Output Example 2

```
1
2
3
4
5
```


## How score is calculated?

The final score consists of two parts. Fifty percent of it is for passing the tests and the other is for the oral presentation.  

The tests score is acheived by running the `run.sh` bash script.  
It requires a unix-like operating system with `bash` and `python3` and `spim` installed on it and.  
***Important***: Since the tests are run usings `spim` your assembly code ***must*** have the main symbol for the simulator to jump into it. This is not needed on mars, hence pay attention to it. Loss of score will occur if your code cannot be run via spim.
For getting a feel on how tests are run change the `quicksort.asm` in line 35 of `run.sh` to `mergesort.asm` and run the script.

***Finally***: Have fun and do not cheat.
