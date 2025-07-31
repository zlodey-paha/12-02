
# Домашнее задание к занятию «Работа с данными (DDL/DML)»

### Задание 1

1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

1.2. Создайте учётную запись sys_temp. 

1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)

1.4. Дайте все права для пользователя sys_temp. 

1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

1.6. Переподключитесь к базе данных от имени sys_temp.

Для смены типа аутентификации с sha2 используйте запрос: 
```sql
ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
```
1.6. По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.

1.7. Восстановите дамп в базу данных.

1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)

*Результатом работы должны быть скриншоты обозначенных заданий, а также простыня со всеми запросами.*

### Решение 1

## Установка MySQL
![Docker](https://github.com/zlodey-paha/12-02/blob/main/Work1/1.1.Docker.PNG)
![SQLInstall](https://github.com/zlodey-paha/12-02/blob/main/Work1/1.2.SQLinstall.PNG)
![DockerRun](https://github.com/zlodey-paha/12-02/blob/main/Work1/1.3.DockerRun.PNG)
![SQL](https://github.com/zlodey-paha/12-02/blob/main/Work1/1.4.SQL.PNG)

## Создание УЗ
![SQLUser](https://github.com/zlodey-paha/12-02/blob/main/Work1/2.SQLUser.PNG)

## Просмотр УЗ
![UserViewer](https://github.com/zlodey-paha/12-02/blob/main/Work1/2%2B3.Create%2BViewerUser.PNG)

## Выдача прав и просмотр прав
![UserPriv](https://github.com/zlodey-paha/12-02/blob/main/Work1/4%2B5.UserPrivileges%2BGrants.PNG)

## Переподключение и смена типа аутентификации
![UserPlugin](https://github.com/zlodey-paha/12-02/blob/main/Work1/6.1.UserPlugin.PNG)

## Скачивание БД
![Download](https://github.com/zlodey-paha/12-02/blob/main/Work1/6.2.1.Download.PNG)
![Unzip](https://github.com/zlodey-paha/12-02/blob/main/Work1/6.2.2.Unzip.PNG)
![Copy](https://github.com/zlodey-paha/12-02/blob/main/Work1/6.2.3.Copy.PNG)

## Восстановление
![DownloadBase](https://github.com/zlodey-paha/12-02/blob/main/Work1/7.1.Download%20base.PNG)
![ShowBase](https://github.com/zlodey-paha/12-02/blob/main/Work1/7.2.ShowBase.PNG)
![ViewerBase](https://github.com/zlodey-paha/12-02/blob/main/Work1/7.3.ViewerBase.PNG)
![ViewerTable](https://github.com/zlodey-paha/12-02/blob/main/Work1/7.4.ViewerTable.PNG)

## ER диаграмма + таблицы
![Schema](https://github.com/zlodey-paha/12-02/blob/main/Work1/8.1.Schema.PNG)
![ViewerTable](https://github.com/zlodey-paha/12-02/blob/main/Work1/8.2.ViewerTable.PNG)

--------------------------------------------------------------------------------------------

### Задание 2

Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: в первом должны быть названия таблиц восстановленной базы, во втором названия первичных ключей этих таблиц. Пример: (скриншот/текст)
```
Название таблицы | Название первичного ключа
customer         | customer_id
```

### Решение 2


------------------------------------------------------------------------------------------

## Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже шире разобраться в материале.

### Задание 3*
3.1. Уберите у пользователя sys_temp права на внесение, изменение и удаление данных из базы sakila.

3.2. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

*Результатом работы должны быть скриншоты обозначенных заданий, а также простыня со всеми запросами.*
