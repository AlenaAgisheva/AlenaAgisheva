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


Для парсинга сайта нам понадобятся библиотеки requests, BeautifulSoup и re.

Первым делом мы должны получить HTML страницу с фильмом. Для этого мы используем библиотеку requests и метод get():

java
```
import requests 

url = 'https://www.kinopoisk.ru/film/535341/'
page = requests.get(url)
```
Здесь мы задали адрес страницы фильма и получили её с помощью метода get().

Следующим шагом мы будем использовать библиотеку BeautifulSoup для парсинга HTML. Мы создадим объект BeautifulSoup из HTML кода страницы фильма:

python
```
from bs4 import BeautifulSoup 

soup = BeautifulSoup(page.content, 'html.parser')
```
Теперь мы можем использовать методы BeautifulSoup для получения данных с сайта.

Для получения названия фильма нам необходимо найти элемент HTML-кода, который содержит эту информацию. Для этого мы воспользуемся методом find() и CSS-селектором:

lua
```
title = soup.find('span', {'class': 'moviename-title-wrapper'}).text.strip()
```
Здесь мы находим элемент span с классом 'moviename-title-wrapper' и получаем текст, содержащий название фильма.

Точно таким же образом мы получим рейтинг и описание фильма:

lua
```
rating = soup.find('span', {'class': 'rating-ball'}).text.strip()

description = soup.find('div', {'class': 'brand_words film-synopsys'}).text.strip()
```
Для получения изображения нам необходимо найти элемент HTML-кода, который содержит ссылку на картинку. Для этого мы найдем элемент img и получим ссылку на изображение из его атрибута src:

csharp
```
image = soup.find('img', {'class': 'moviename-poster'}).get('src')
```
Теперь мы можем вывести полученную информацию:

python
```
print('Title:', title)
print('Rating:', rating)
print('Description:', description)
print('Image:', image)
```

Полную версию программы можно увидеть здесь:

lua
```
import requests
from bs4 import BeautifulSoup

url = 'https://www.kinopoisk.ru/film/535341/'
page = requests.get(url)
soup = BeautifulSoup(page.content, 'html.parser')

title = soup.find('span', {'class': 'moviename-title-wrapper'}).text.strip()
rating = soup.find('span', {'class': 'rating-ball'}).text.strip()
description = soup.find('div', {'class': 'brand_words film-synopsys'}).text.strip()
image = soup.find('img', {'class': 'moviename-poster'}).get('src')

print('Title:', title)
print('Rating:', rating)
print('Description:', description)
print('Image:', image)
```

