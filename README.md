<a id = "anchor"></a>
# API Yamdb — программный интерфейс для сбора отзывов и составления рейтингов произведений

### Описание

Программный интерфейс создан, как платформа для размещения отзывов и составления рейтингов произведений по категориям. При запуске проекта доступны категории "Книги", "Фильмы", "Музыка". Список может быть расширен или изменен из админ-зоны сайта. Функционал интерфейса предусматривает возможность не только размещать отзывы и ставить оценки произведениям, но и оставлять комментарии к отзывам других пользователей. Для регистрации необходимо ввести логин и адрес своего почтового ящика, после чего отправить код подтверждения и в ответе от сервиса придет JWT-токен, который обеспечит доступ ко всему пользовательскому функционалу сайта. Неавторизованным пользователям сервис доступен только для чтения. Сервис предусматривает 4 уровня идентификации пользователей: аноним, юзер, модератор и админ. Каждый из уровней имеет соотвествующие доступы к приложениям сервиса для их релевантного использования и обеспечения безопасной эксплуатации. 
***
### Технологии
* Python 3.8.3 
* Django 2.2.16 
* djangorestframework 3.12.4 
* PyJWT 2.1.0  
Полный список используемых технологий -> requirements.txt
***
### Запуск проекта в dev-режиме
клонируйте репозиторий 
```
git clone git@github.com:andrey-kolesnik-moscow/api_yamdb.git
```
создайте и активируйте виртуальное окружение
```
python3 -m venv venv
```
для Windows
```
source venv/Scripts/activate
```
для macOS или Linux
```
source venv/bin/activate
```
установите зависимости проекта
```
pip install -r requirements.txt
```
выполните миграции
```
python3 manage.py migrate
```
отдельно можете импортировать тестовые данные
```
python3 manage.py import_csv
```
запустите проект на локальной машине 
```
python3 manage.py runserver 
```
***
Документация к проекту доступна сразу после запуска сервера  ` /redoc/ `  
***
### Авторы
* Андрей Колесник
* Георгий Кузнецов
* Павел Фирсов
***
[В начало страницы](#anchor)

