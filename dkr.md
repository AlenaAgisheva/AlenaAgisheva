1. Написать алгоритм сортировки вставками 
2. def insertion_sort(arr):
3.  for i in range(1, len(arr)):
4.    key = arr[i]
5.    j = i - 1
6.    while j >= 0 and key < arr[j]:
7.      arr[j + 1] = arr[j]
8.      j -= 1
9.    arr[j + 1] = key
10. return arr 
