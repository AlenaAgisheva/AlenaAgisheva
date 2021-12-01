# Лабораторная работа 13
# Задача 1. 
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if abs(x1-x2) <=1 and abs(y1-y2) <=1:
    print('YES')
else:
    print('NO')
    
# Задача 2.
a = int(input())
b = int(input())
c = int(input())
if a == b == c:
    print('Равносторонний')
if a == b or b == c or a == c:
    print('Равнобедренный')
else:
    print('Разносторонний')
   
# Задача 3.
a1 = int(input())
b1 = int(input())
a2 = int(input())
b2 = int(input())
a3 = max(a1, a2)
b3 = max(b1, b2)
if a3 < b3:
    print(a3, b3)
elif a3 == b3:
    print(a3)
else:
    print('Пустое множество')
    
