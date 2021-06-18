

Laravel Log Viewer
============

This Package can be used to show laravel log files inside of a web page using Bootstrap and DataTables. it can be used with Laravel/Lumen 4.2+ all the way through to the lastest versions.
this package is a fork from the famous [Log-Viewer](https://github.com/rap2hpoutre/laravel-log-viewer) package with minor changes.


### Requirements
- PHP 5.4+
- Laravel 4.2+


### Installation

#### Composer Install:

	composer require alibayat/laravel-logviewer

#### Publish configuration:

```bash
php artisan vendor:publish \
  --provider="AliBayat\LaravelLogViewer\LaravelLogViewerServiceProvider"

```

#### Publish view file:

```bash
php artisan vendor:publish \
  --provider="AliBayat\LaravelLogViewer\LaravelLogViewerServiceProvider" \
  --tag=views


```

---

### Usage

you can use any route you want to point to the index method of the controller included in the package:

```php

Route::get('logs', '\AliBayat\LaravelLogViewer\LogViewerController@index');

```


#### Credits

 - Ali Bayat - <ali.bayat@live.com>
