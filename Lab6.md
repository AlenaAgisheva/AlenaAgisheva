# Лабораторная работа №11

# 1 задание
```
print('Агишева Алена Владимировна')
print('Р20Б1, Радиотехнический факультет, ВИ МВД')
```

# 2 задание
```
print('I', 'like', 'Python', sep='***')
```

# 3 задание
```
a = input()
b = input()
c = input()
d = input()
print(b, c, d, sep=a)
```

# 4 задание
```
name = input()
print('Привет, ', name, '!', sep='')
```

# Лабораторная работа №12

## 1 Задание.
```
n = int(input())
print('1 число - ', n//1000)
print('2 число - ', (n//100)%10)
print('3 число - ', (n//10)%10)
print('4 число - ', n%10)
```

## 2 Задание. Вариант 2.
```
x = float(input())
from math import *
print(e ** ((2 ** (1/2))/(sin(x)))+3*x**2-1)
```
## 3 Задание. 
```
import math
 
print("Введите коэффициенты для уравнения")
print("ax^2 + bx + c = 0:")
a = float(input("a = "))
b = float(input("b = "))
c = float(input("c = "))
 
d = b ** 2 - 4 * a * c
print("Дискриминант D = %.2f" % d)
 
if d > 0:
    x1 = (-b + math.sqrt(d)) / (2 * a)
    x2 = (-b - math.sqrt(d)) / (2 * a)
    print("x1 = %.2f \nx2 = %.2f" % (x1, x2))
elif d == 0:
    x = -b / (2 * a)
    print("x = %.2f" % x)
else:
    print("Корней нет")
```
