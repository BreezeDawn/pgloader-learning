# pgloader with docker-compose running

## command lines

* from csv 2 pg

```code
docker-compose up -d postgres
docker-compose up pgloader-csv
```

* from fixed columns 2 pg

```code
docker-compose up -d postgres
docker-compose up pgloader-fixed
```

* from mysql 2 pg

```code

for mysql:

mysql -uroot  -h127.0.0.1 -pdalongrong
create database f1db;
use f1db
source init-db/mysql/f1db.sql

for pg you may need create database f1db

docker-compose up pgloader-mysql
```