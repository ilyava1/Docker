Задание №1

1. Собрать образ из директории task_1:
   docker image build ./task_1 --tag=greeting

2. Запустить контейнер:
   docker run --name=task_1 -p 7007:80 -d greeting

3. Проверить страницу приветствия:
   сurl localhost:7007/

------------------------------------------------------------------

Задание №2

1. Собрать образ из директории task_2/stocks_products:
   docker image build . --tag=stocks_products

2. Запустить контейнер:
   docker run --name=task_2 -p 7008:6060 -d stocks_products

3. Проверить работу API:
   открыть файл task_2/stocks_products/requests-examples.http в VSC, инициировать запросы:
	- Создание продукта
	- Получение продуктов