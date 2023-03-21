# CMPS 2200 Reciation 5
## Answers

**Name:** Sydney Feldman


Place all written answers from `recitation-06.md` here for easier grading.







- **1b.**

SORTED:

|     n |   qsort-fixed-pivot |   qsort-random-pivot |    ssort |
|-------|---------------------|----------------------|----------|
|    10 |               0.001 |                0.007 |    0.014 |
|    20 |               0.000 |                0.003 |    0.025 |
|    50 |               0.000 |                0.001 |    0.113 |
|   100 |               0.000 |                0.002 |    0.363 |
|   200 |               0.000 |                0.003 |    3.217 |
|   500 |               0.001 |                0.005 |    8.948 |
|  1000 |               0.001 |                0.004 |   58.818 |
|  2000 |               0.002 |                0.014 |  252.809 |
|  5000 |               0.002 |                0.015 | 1897.388 |
| 10000 |               0.002 |                0.016 | 5853.319 |


UNSORTED: 
|     n |   qsort-fixed-pivot |   qsort-random-pivot |    ssort |
|-------|---------------------|----------------------|----------|
|    10 |               0.001 |                0.003 |    0.016 |
|    20 |               0.000 |                0.001 |    0.026 |
|    50 |               0.001 |                0.002 |    0.118 |
|   100 |               0.000 |                0.002 |    0.548 |
|   200 |               0.001 |                0.003 |    1.534 |
|   500 |               0.001 |                0.003 |    8.242 |
|  1000 |               0.001 |                0.003 |   79.341 |
|  2000 |               0.001 |                0.005 |  234.998 |
|  5000 |               0.002 |                0.006 | 1652.200 |
| 10000 |               0.002 |                0.006 | 6732.908 |


The running times are similar to the asymptotic bounds. This is shown as selection short has the worst asymptotic runtime of the three. When the input size increases, the running time increases significantly when using selection sort, and only minimally when using quick sort. Both verisons of quicksort are faster than selection sort. When the input list is sorted, the selection sort times are a bit faster, but not significantly faster. However, the quick sort times are actually slower when the list is already sorted. 

- **1c.**
Unsorted
|     n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sort |
|-------|---------------------|----------------------|------------|
|    10 |               0.001 |                0.004 |      0.003 |
|    20 |               0.000 |                0.002 |      0.002 |
|    50 |               0.000 |                0.002 |      0.005 |
|   100 |               0.000 |                0.002 |      0.012 |
|   200 |               0.000 |                0.002 |      0.021 |
|   500 |               0.001 |                0.002 |      0.087 |
|  1000 |               0.001 |                0.003 |      0.153 |
|  2000 |               0.001 |                0.003 |      0.283 |
|  5000 |               0.002 |                0.006 |      0.944 |
| 10000 |               0.002 |                0.005 |      1.938 |

Even though Timsort is significantly faster than selection sort, both quick sort implementations are faster than timsort. If it was sorted, the tim_sort times would be faster than they are here. 