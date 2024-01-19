# FirstDjango_150124

## Инструкция по развертыванию проекта
1. `python3 -m venv django_venv`

2. `source django_venv/bin/activate`

3. `pip install -r requirements.txt`

4. `python manage.py migrate`

5. `python manage.py runserver`

## Запуск терминала в контексте **django**
`python manage.py shell_plus --ipython`


## Выгрузка и загрузка данных из БД
Выгрузка данных для приложения MainApp:  
`python manage.py dumpdata MainApp --indent 4 > ./datasets/items.json`

Выгрузка данных из таблицы:  
`python manage.py dumpdata MainApp.item --indent 4 > ./datasets/items.json`

Загрузка данных:  
`python manage.py loaddata ./datasets/items.json`