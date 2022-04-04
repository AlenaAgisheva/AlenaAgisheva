## Flask bootstrap

В новом проекте создаем файл app.py 

Установка flack производится через терминал 
установка python3 -m pip install flask_bootstrap
прведем код к виду

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

создадим каталог(directory) templates, а в нем создадим файл index.html
отредактируем файл, добавив в него следующую строчку
{% extends "bootstrap/base.html" %}

Пробуем запустить сервер. Если сервер не запускается
deactivate and activate the virtual environment solved it
deactivate . venv/bin/activate
снова запустите
должна отобразиться пустая страница
нажмите клавише F12 либо ПКМ-> просмотреть код страницы, убедитесь что flask-bootsrap подключен
