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
def rectangle_area(self, length, width):
    return length*width

def rectangle_perimeter(self, length, width):
    return 2*(length+width)

def square_area(self, side):
    return side**2

def square_perimeter(self, side):
    return 4*side

def circle_area(self, radius):
    return 3.14*radius**2

def circle_perimeter(self, radius):
    return 2*3.14*radius

def triangle_area(self, base, height):
    return 0.5*base*height

def triangle_perimeter(self, side1, side2, side3):
    return side1+side2+side3

Пример использования класса
gf = GeometricFigures()

print(gf.rectangle_area(5, 10))
print(gf.rectangle_perimeter(5, 10))
print(gf.square_area(5))
print(gf.square_perimeter(5))
print(gf.circle_area(5))
print(gf.circle_perimeter(5))
print(gf.triangle_area(5, 10))
print(gf.triangle_perimeter(5, 8, 10))
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

