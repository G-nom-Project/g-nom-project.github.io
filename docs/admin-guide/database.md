
!!! example "Database containers"
    A database container will be included in the `docker-compose` file released with the new [installation guide](../setup.md). Migrations will be performed automatically.

While Laravel provides database drivers for a selection of relational databases, we recommend using PostgreSQL.

Once the database server is set up, run the migrations once to create all required tables:
```
php artisan migrate
```