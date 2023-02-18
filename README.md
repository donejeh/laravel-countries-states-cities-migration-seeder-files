##  Countries States Cities Database migration and seeders for laravel.


All Countries, States & Cities are Covered & Populated for you to use in your Laravel project
- Total number of 250 Countries
- Total number of 4989 states
- Total number of 150710 cities
## how to use:

copy this files from migrations and seeders to your project seeder project 

- Run
```
php artisan migrate
```

Enjoy...

## Error you may see and fixes

- datetime value: '0000-00-00 00:00:00' for column 'created_at' at row 1")

to it this just change your:

$table->timestamps();  

to 

$table->string('created_at')->nullable();
$table->string('updated_at')->nullable();

- Allowed memory size of 536870912 bytes exhausted (tried to allocate 77710688 bytes) laravel

change your memory_limit in php.ini

; Old Limit
; memory_limit = 512M

; New Limit
memory_limit = 2048M
