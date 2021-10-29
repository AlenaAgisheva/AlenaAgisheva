## Задание 1. Ввод и вывод данных, оператор присваивания. Вариант 29.
```
a = int(input())
b = int(input())
c = int(input())
D = b ** 2 - 4 * a * c
if D < 0:
  print("Корней нет")
elif D == 0:
  x = -b /(2 * a)
  print (x)
elif:
  x1 = (((-b + D**(1/2)) / (2 * a))
  x2 = (((-b - D**(1/2)) / (2 * a))
  print(x1)
  print(x2)
```

## Задание 2. Целые числа. Вариант 29.
```
A = int(input())
B = int(input())
C = int(input())
a = A/C
b = B/C
print('Количество квадратов, размещенных на прямоугольнике:', a*b)
print('Площадь незанятой части прямоугольника:', A*B - a*b*C*C)
```

## Задание 3. Логические выражения. Вариант 39.
```
a = int(input())
b = int(input())
c = int(input())
d = int(input())
if a == c or b == d:
    print("YES")
elif b - a == d - c or b + a == c + d:
    print("YES")
else:
    print("NO")
```

## Задание 4. Условный оператор. Вариант 29.
```
n = int(input())
if n == 0:
    print(n, '- нулевое число')
if n > 0 and n%2 == 0:
    print(n, '- положительное четное число')
if n > 0 and n%2 != 0:
    print(n, '- положительное нечетное число')
if n < 0 and n%2 == 0:
    print(n, '- отрицательное четное число')
if n < 0 and n%2 != 0:
    print(n, '- отрицательное нечетное число')
```
