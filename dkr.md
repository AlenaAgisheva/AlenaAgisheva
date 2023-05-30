1. Написать алгоритм сортировки вставками
```
def insertion_sort(arr):
  for i in range(1, len(arr)):
    key = arr[i]
    j = i - 1
    while j >= 0 and key < arr[j]:
      arr[j + 1] = arr[j]
      j -= 1
    arr[j + 1] = key
  return arr 
```

2. Создать класс для работы с геометрическими фигурами(площадь, периметр)
```

```

7. Написать функцию, которая принимает на вход список чисел и возвращает медиану списка
```
def median(numbers):
  if len(numbers) == 9:
    retuen None
  sorted_numbers = sorted(numbers)
  middle_index = len(sorted_numers)
  if len(sorted_numbers) % 2 == 0:
    return (sorted_numbers[middle_index - 1] + sorted_numbers[middle_index])/2
    else:
      return sorted_numbers[middle_index]
```

