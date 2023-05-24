# Dockerizing Flask with Postgres, Gunicorn, and Nginx  
Готовый код [учебного проекта](https://testdriven.io/blog/dockerizing-flask-with-postgres-gunicorn-and-nginx/) по контейнеризации Flask приложения.  
Для построения необходимо установить Docker и Docker-compose


В этом репозитории два варианта сборок: Production и Development  
Для сборки **Dev.** варианта - ввод команды:  
`docker-compose up -d --build`

Для сборки **Prod.** варианта - ввод команды:  
`$ docker-compose down -v` - для остановки запущенных контейнеров

`$ docker-compose -f docker-compose.prod.yml up -d --build` - для сборки и запуска контейнеров 


`$ docker-compose -f docker-compose.prod.yml exec web python manage.py create_db` - выполнение CLI команды

