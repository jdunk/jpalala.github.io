
Laravle Cheatsheet
====

Artisan commands
---

List artisan commands:

`php artisan list`

See help about migrate:

`php artisan help migrate`

Create a controller:

`php artisan make:controller TodoController`

Create a model and migration : 

`php artisan make model Todo -m`

Create a migration and set a custom table

`php artisan make:migration add_todos_to_db --table=todos

Run your migrations:

`php artisan migrate`

Tinker with your app (to do some debuging):

`php artisan tinker`

 

Renaming adding a column 

`php artisan make:migration add_column_name_to_users --table="users"`


