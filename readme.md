# How to setup a webserver in go

Tutorial: https://www.lynda.com/Go-tutorials/Replacing-default-template-engine/516402/516855-4.html

## run the server

go run main.go

http://localhost:8080/

## setup webserver negroni

go get github.com/codegangsta/negroni

## Setup db

$ go get github.com/mattn/go-sqlite3

$ sqlite3 dev.db

sqlite> .schema

CREATE TABLE books(
pk integer primary key autoincrement,
title text,
author text,
id text,
classification text);

sqlite> select * from books;

sqlite> .exit

## html template render

go get github.com/yosssi/ace

## http route

go get github.com/gorilla/mux