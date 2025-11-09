G-nom uses [Laravel worker queues](https://laravel.com/docs/12.x/queues) for long-running background tasks such as [imports](../user-guide/import.md). In short, workers are launched using artisan in a php-evironment:
```bash
php artisan queue:work --timeout=120
```
While it is possible to run the worker direcly on the host system, it's recommended to launch docker worker containers mounted to the G-nom installation directory.

!!! example "Worker containers"
    Worker containers will be included in the `docker-compose` file released with the new [installation guide](../setup.md).

## Dispatching jobs
Jobs can be launched manually using tinker, the following detail shows the process for re-building the taxon table based on a new NCBI taxdmp release:
```

$ php artisan tinker
Psy Shell v0.12.9 (PHP 8.4.13 — cli) by Justin Hileman
> use App\Jobs\RebuildTaxonTable;
> RebuildTaxonTable::dispatch(2);
= Illuminate\Foundation\Bus\PendingDispatch {#6671}

```