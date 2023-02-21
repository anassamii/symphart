Setup:
php 7.3.28
run xampp
modify .env
composer update
composer install ?
maybe some other installations
(didn't work) php bin/console doctrine:migrations:diff
(didn't work) php bin/console doctrine:migrations:migrate
(I replaced them with this :) php bin/console doctrine:schema:update --force (to create table(s))
symfony server:start


entity = model
Laravels routes # symfonys routes
Laravels syntaxe # Symfonys syntaxe
OOP: we use Getters and Setters in case we declare varibales "private"


Define an enity (table):
php bin/console make:entity <Name(capital)>

Create entities in DB (tables) || After modifying entity(ies) file:
php bin/console doctrine:migrations:diff
php bin/console doctrine:migrations:migrate
Or use this: php bin/console doctrine:schema:update --force


# SymphArt

> A basic Symfony 4 CRUD application used in the tutorial series "Up & Running With Symfony 4"

## Quick Start

``` bash
# Install dependencies
composer install

# Edit the env file and add DB params

# Create Article schema
php bin/console doctrine:migrations:diff
# Run migrations
php bin/console doctrine:migrations:migrate

# Build for production
npm run build

# Run symfony server 
symfony server:start

```

## App Info

### Author

Brad Traversy
[Traversy Media](http://www.traversymedia.com)

### Version

1.0.0

### License

This project is licensed under the MIT License
