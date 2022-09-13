## Installation

```shell
git clone https://github.com/laragis/laravel.git -b auth laravel-auth
cd laravel-auth

docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php81-composer:latest \
    composer install --ignore-platform-reqs
    
./vendor/bin/sail up
```
