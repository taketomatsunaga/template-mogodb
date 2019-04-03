# MongoDB

- MongoDB version 3.4

## Build

```sh

docker build -t my-mongodb:0.0.1 .

```

## Configure

Change username and password for root user if you need in `Dockerfile`.


 ```

 ENV MONGO_INITDB_ROOT_USERNAME root
 ENV MONGO_INITDB_ROOT_PASSWORD mongo

 ```


## Run

```sh

docker run -d -it -p 27017:27017 my-mongodb:0.0.1

```
## Connect From Tool

Install `NoSQLBooster for MongoDB` from [here](https://nosqlbooster.com/downloads).
And connect with the configuration below and create a database.


```
host=localhost
port=27017
user:root
password:mongo
```

## Connect From App

```

uri: "mongodb://@localhost:27017/{database name}"

```
