<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## langkah instalasi

1. buat file .env
2. set pengaturan database
3. $php artisan make:auth
4. copy folder
    /app/helpers/
    /app/Http/Controller/
    /app/Models/
    /database/migrations
    /public/
    /resources/views

5. composer require box/spout
6. composer require barryvdh/laravel-dompdf
    * set file /config/app.php
    - Barryvdh\DomPDF\ServiceProvider::class,
    - 'PDF' => Barryvdh\DomPDF\Facade::class,
7. copy file /public/.htaccess ke root folder
8. ubah nama file server.php pada root folder menjadi index.php
9. edit file /Illuminate/Routing/UrlGenerator.php
  <!-- public function asset($path, $secure = null)
  {
     ......
     return $this->removeIndex($root).'/'.trim($path, '/');
  }
  - menjadi
  public function asset($path, $secure = null)
  {
     ......
     return $this->removeIndex($root).'/public/'.trim($path, '/');
  } -->

copy isi file
  - /routes/api.php
  - /routes/web.php

* ikuti langkah https://commit-cyber.com/stories/powerful-real-time-web-applications-dengan-laravel-react-socketio-redis-vyMhpihbQW
