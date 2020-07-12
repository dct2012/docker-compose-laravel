Docker Compose Laravel
====
Docker Compose environment with Laravel 7.4.3 preinstalled under `_laravel`. 
Alternatively, install your own copy of laravel under `_laravel`. 
Maybe one day move Laravel install/setup to composer based.

Usage
-----

1. bring your instance up: \
```$ docker-compose up -d```

1. install php dependencies: \
```$ docker exec -it laravel-app /bin/bash``` \
```$ composer install```

1. While still inside the container generate an app key: \
```$  php artisan key:generate```

1. Copy `_laravel/.env.example` to `_laravel/.env` and edit appropriately.

1. Visit: http://localhost/

1. take your instance down: \
```$ docker-compose down```

Considerations
----
1. Laravel