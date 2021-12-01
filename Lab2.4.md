# Лабораторная работа 14
## Задание 1
```
a = 1
x = 3
for n in range(0, 30):
    a += (3n+2)*x**(n-1)
    print(a) 
```

## Задание 2
```
x = input().split()
sum = 0
for i in x:
    sum += int(i)
print('Сумма всех чисел последовательности: ', sum)   
```

## Задание 3
```
a = input().split()
pos = 0
neg = 0
for i in a:
    if int(i) > 0:
        pos += int(i)
    elif int(i) < 0:
        neg += int(i)
    else:
        break
print('Сумма положительных чисел: ', pos)
print('Сумма отрицательных чисел: ', neg)    
```
