#1 Установка Laravel 

https://laravel.com/docs/8.x/installation

```php 
composer create-project laravel/laravel example-app
```

#2 IDE Helper

https://github.com/barryvdh/laravel-ide-helper

```
composer require --dev barryvdh/laravel-ide-helper
```

* использование

```
php artisan ide-helper:generate //- PHPDoc generation for Laravel Facades
php artisan ide-helper:models //- PHPDocs for models
php artisan ide-helper:meta //- PhpStorm Meta file
```

* добавляем в файл composer.json в секцию scripts следующий массив

```
"post-update-cmd": [
        "Illuminate\\Foundation\\ComposerScripts::postUpdate",
        "@php artisan ide-helper:generate",
        "@php artisan ide-helper:meta"
    ]
```


#3 Debugbar

https://github.com/barryvdh/laravel-debugbar

```
composer require barryvdh/laravel-debugbar --dev
```

#4 Laravel UI

https://github.com/laravel/ui

```
composer require laravel/ui
```

* использование

```
// Generate basic scaffolding...
php artisan ui bootstrap
php artisan ui vue
php artisan ui react

// Generate login / registration scaffolding...
php artisan ui bootstrap --auth
php artisan ui vue --auth
php artisan ui react --auth
```

#5 Node

https://nodejs.org/en/download/

```
npm install
npm run dev
```

#6 Настройка .env

#7 Создание миграций

```
php artisan migrete
```


