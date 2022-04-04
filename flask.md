## Flask bootstrap

Установка flask_bootstrap производится через терминал командой pip install flask_bootstrap
 
В новом проекте создаем файл app.py , прведем код к виду:
```
from flask import Flask
from flask import render_template
from flask_bootstrap import Bootstrap

app = Flask(__name__)
Bootstrap(app)

@app.route("/")
def index():
  return render_template('index.html')
  
if __name__ == '__main__':
app.run(debug = True)
```
 
После чего создаем directory (каталог) templates (с другим названием flask может работать некорректно), а в нем создадим файл index.html
! Если после создания html файла базовая структура не отображается, то выводим ее, написав ! и нажимая tab
```
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>

</body>
</html>
```
Отредактируем файл, добавив в него следующую строчку {% extends "bootstrap/base.html" %}

Пробуем запустить сервер. Если сервер не запускается:
deactivate and activate the virtual environment solved it
deactivate . venv/bin/activate
Снова запустите, должна отобразиться пустая страница. Нажмите клавишу F12 либо ПКМ -> просмотреть код страницы, убедитесь что flask-bootsrap подключен.

Для того, чтобы вывести шаблон HTML страницы, 
