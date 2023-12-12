# Docker dev environment for laravel 10

## Setup

copy files or clone repo into your main project folder in the same directory where you have composer.json

1. build containers
    docker compose build -d

2. enter app container
    docker exec -it app bash

3. run commands in app container to build composer and node packages
    composer install
    php artisan migrate
    php artisan db:seed

    npm install
    npm run build
