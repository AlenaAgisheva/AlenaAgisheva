# Задание 1. Цикл с параметром. Вариант 34.

```
n = int(input())
A1 = 1
A2 = 2 
A3 = int()
print("A1 =", A1)
print("A2 =", A2)
for i in range(3, n+1):
    A3 = (A1 + 2*A2)/3
    print("A", i, "=", A3)
    A1 = A2
    A2 = A3
```

# Задание 2. Цикл с условием. Вариант 2.

```
A = int(input())
B = int(input())
print('A =', A)
print('B =', B)
r = A - B 
n = 1 
while r >= B:
    r -= B 
    n += 1 
print('Количество размещений B в A: ', n)
print('Остаток: ', r)
```

# Задание 3. Цикл с условием. Вариант 39.

```
n = int(input())
b = 1/10 ** n
A1 = 1
A2 = 2 
A3 = (A1 + 2*A2)/3
print('A1=', A1)
print('A2=', A2)
print('A3=', A3)
k = 3 
while abs(A3 - A2) >= b:
    A2, A3=A3, (A2 + 2*A3)/3
    k += 1
    print('A', k, '=', A3)
print(k, '=', A2, ',', k-1, '=', A3)
```
