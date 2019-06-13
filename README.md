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

* from pg 2 pg

```code

```