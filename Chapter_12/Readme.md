####Chapter 12

> As you'll learn in this chapter, less and more allow you to view the contents of files.
> Alternative "english" ways of asking for your working directory:

```
Evidently this Chapter is predicated on a Rails application running on the
machine.
```

> Can we see what's in our production log?

```
Yes, provided one existed on this Mac. I have a Rails development log
on another machine and it contains a record of sql commands, routing actions, 
and other activities relavent to Rails operations.

Here's a sample of what it contains:

Started GET "/ostapp/intro/dynamic" for 24.216.71.14 at Fri May 15 16:04:13 -0500 2015
  Processing by IntroController#dynamic as HTML
Rendered intro/dynamic.html.erb within layouts/application (10.0ms)
Completed 200 OK in 23ms (Views: 21.3ms | ActiveRecord: 0.0ms)
  ESC[1mESC[36mSQL (4.1ms)ESC[0m  ESC[1m SELECT name
 FROM sqlite_master
 WHERE type = 'table' AND NOT name = 'sqlite_sequence'
ESC[0m
  ESC[1mESC[35mSQL (0.2ms)ESC[0m  select sqlite_version(*)
  ESC[1mESC[36mSQL (7.8ms)ESC[0m  ESC[1mCREATE TABLE "schema_migrations" ("version" varchar(255
) NOT NULL) ESC[0m
```

> What does our database.yml look like?

```
The database.yml (from another machine) appears to specify the database and 
some performance metrics relavent to database ops.
```


```
Brookss-MBP:config $ cat database.yml
# SQLite version 3.x
#   gem install sqlite3-ruby (not necessary on OS X Leopard)
development:
  adapter: sqlite3
  database: db/development.sqlite3
  pool: 5
  timeout: 5000

# Warning: The database defined as "test" will be erased and
# re-generated from your development database when you run "rake".
# Do not set this db to the same as development or production.
test:
  adapter: sqlite3
  database: db/test.sqlite3
  pool: 5
  timeout: 5000

production:
  adapter: sqlite3
  database: db/production.sqlite3
  pool: 5
  timeout: 5000
```
