####Chapter 12

> As you'll learn in this chapter, less and more allow you to view the contents of files.
> Alternative "english" ways of asking for your working directory:

```
Evidently this Chapter is predicated on a Rails application running on the
machine.
```

> Can we see what's in our production log?

```
Brookss-MBP:learn_command_line_exercises $ less /Users/bi/OReilly\ Ed/school\ download/railsapps\ \(copy\)/ostapp/log/development.log

(sample screen of less editor)

 WHERE type = 'table' AND NOT name = 'sqlite_sequence'
ESC[0m
  ESC[1mESC[35mSQL (1.7ms)ESC[0m   SELECT name
 FROM sqlite_master
 WHERE type = 'table' AND NOT name = 'sqlite_sequence'
  ESC[1mESC[36mSQL (1.7ms)ESC[0m  ESC[1mSELECT "schema_migrations"."version" FROM "schema_migrations"ESC[0m
Migrating to CreateTasks (20150515210149)
Migrating to CreatePhotos (20150515213630)
  ESC[1mESC[35mSQL (1.0ms)ESC[0m  select sqlite_version(*)
  ESC[1mESC[36mSQL (2.8ms)ESC[0m  ESC[1mCREATE TABLE "photos" ("id" INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL, "caption" varchar(255), "description" text, "url" varchar(255), "rating" integer, "created_at" datetime, "updated_at" datetime) ESC[0m
  ESC[1mESC[35mSQL (0.1ms)ESC[0m  INSERT INTO "schema_migrations" ("version") VALUES ('20150515213630')
  ESC[1mESC[36mSQL (1.9ms)ESC[0m  ESC[1m SELECT name
 FROM sqlite_master
 WHERE type = 'table' AND NOT name = 'sqlite_sequence'
ESC[0m
  ESC[1mESC[35mSQL (1.6ms)ESC[0m  SELECT "schema_migrations"."version" FROM "schema_migrations"
  ESC[1mESC[36mSQL (1.8ms)ESC[0m  ESC[1m SELECT name
 FROM sqlite_master
 WHERE type = 'table' AND NOT name = 'sqlite_sequence'
ESC[0m
  ESC[1mESC[35mSQL (0.1ms)ESC[0m  PRAGMA index_list("photos")
  ESC[1mESC[36mSQL (0.1ms)ESC[0m  ESC[1mPRAGMA index_list("tasks")ESC[0m


Started GET "/ostapp/photos/" for 72.42.74.242 at Fri May 15 16:40:03 -0500 2015
  Processing by PhotosController#index as HTML
  ESC[1mESC[35mPhoto Load (3.5ms)ESC[0m  SELECT "photos".* FROM "photos"
Rendered photos/index.html.erb within layouts/application (7.3ms)
Completed 200 OK in 41ms (Views: 30.6ms | ActiveRecord: 13.4ms)


:
```

> What does our database.yml look like?

```
Brookss-MBP:learn_command_line_exercises $ more /Users/bi/OReilly\ Ed/school\ download/railsapps.hosed/ostapp/config/database.yml

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
