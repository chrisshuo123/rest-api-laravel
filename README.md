# Introduction
This repository purpose is to re-train my REST-API ability via Laravel, using Laravel version 11.  As a reference, I learn on how to manage REST API via 'Santri Coding', an Indonesian Developer that teaches us on how to code via Laravel, PHP, JavaScript, and any other stacks. <br>

You can find his link right here, he offer lots of tutorials whether its free or the payed version:<br>
[Santri Koding Website](https://santrikoding.com/)

For the tutorials I've enrolled in Santri Coding, here's the link to the complete text-based tutorials:<br>
[How to create REST API Laravel Installation *(Tutorial Restful API Laravel 11)*](https://santrikoding.com/tutorial-set/tutorial-restful-api-laravel-11?from=live-search)<br>

If you guys are more comfortable with Video learning based _(primarily for begineer programmers)_, then you might access the video REST API Laravel Tutorial:<br>
[Tutorial Restful API Laravel 11](https://youtube.com/playlist?list=PL-2rLYVN9WCw34_TXFwl84r7DW9vwnj5s&si=HTgyl4iIU37p1Lna)

## Getting Started
Complete Explanation on How to set-up Laravel from Zero: [Tutorial Restful API Laravel 11](https://youtube.com/playlist?list=PL-2rLYVN9WCw34_TXFwl84r7DW9vwnj5s&si=HTgyl4iIU37p1Lna) <br>
**Note:** Please take note that this uses Indonesian language.  To make it easy, I'll explain in english using simple words and with some tutorials modified by myself, primarily for the Laragon.<br>

From the link on [santrikoding.com](https://santrikoding.com) above (which is spoken in Indonesian Language), here's what you need:
- Laragon
- Composer
- VSCode
- PHP Extension setup _(after laragon installed)_<br>

If you don't have Laragon, here's the link to it:<br>
[Laragon Download Link](https://laragon.org/download) <br>
**What is Laragon?** In a Nutshell, it's like the XAMPP for the PHP, which is more efficient & all-in-one with instant switch button _(like turning on the Apache and MySQL Module on xampp)_, root web button _(Instantlly brings you toward the root directory web)_, database _(Instantlly opens the HeidiDB, think of it as your localhost/phpmyadmin xampp, or the MySQL Workbench IDE)_, terminal _(built-in cmd for laravel)_, and the Root _(brings you instantlly toward the 'C:/laragon/www/' directory, same like in 'xampp/htdocs' for PHP)_.
<br><br>
If you don't have Composer, here's the link to install:<br>
[getcomposer download link](https://getcomposer.org/download/)<br>

**How to download?** There are several ways to download & install composer:<br>
1. [How to Install Composer on Windows only 1 Minutes](https://www.youtube.com/shorts/wUkeoz28NY8)
2. [How to Install Composer on Mac only 1 Minutes](https://www.youtube.com/watch?v=_gJ_7Y5THGY)
<br>

**If you don't have VSCode?** Download via this link: [visual studio code download](https://code.visualstudio.com/download)<br>
Pick a choice to download according to software you're using, _whether its a windows, mac os, or linux_.
<br>

**For the Extension?** Here are the list of PHP Extension given from the tutor: <br>
_**For those Confused:** This extensions aren't those in VSCode, but from the php.ini laragon, similar to xampp/php/php.ini for the native php version._<br>
- extension=bcmath
- extension=ctype
- extension=json
- extension=mbstring
- extension=openssl
- extension=pdo_mysql
- extension=tokenizer
- extension=xml<br>
For Laragon, go to _C:\laragon\bin\php\php-XXversionXX\php.ini_, to enable those extensions.  Make sure to double check using CTRL + F, and search the points given above one-by-one to makesure the extensions are included.  If haven't included, copy & paste into the php.ini above the other 'extension=' line that exists.  If already included, just simple erase the ';' to enable the php extension.<br><br>

## For the full Tutorial

### SantriKoding Laravel #1 - How to Install and Run Laravel 11: 
Text-based Tutorial Link: [Tutorial Restful API Laravel 11 #1: How to make REST API Laravel & Installation _(Tutorial Restful API Laravel 11 #1: Cara Install & Menjalankan Laravel 11)_](https://santrikoding.com/tutorial-restful-api-laravel-11-1-cara-install-menjalankan-laravel-11) <br>
Video-based Tutorial Link: [Tutorial Restful API Laravel 11 #2: How to Install & Run Laravel 11 _(Tutorial Restful API Laravel 11 #2: Cara Install & Menjalankan Laravel 11)_](https://www.youtube.com/watch?v=5CqaQTeSHTw&list=PL-2rLYVN9WCw34_TXFwl84r7DW9vwnj5s&index=2)<br>
**Please be advice:** This tutorial are spoken in Indonesian language.  For Simplicity, I'll guide you using simple English Language.<br><br>

**Branch: 'part1_modelAndMigration'**<br><br>

#### Simple explanation in English
For me myself, the Extensions that I've installed is only the OpenSSL.<br>
To create the laravel file _(from my own version)_:
1. Open the Laragon
2. Click on the 'Terminal' Button<br>
3. In terminal, type 'composer create-project --prefer-dist laravel/laravel:^11.0 laravel-api'.  This will create a new project named 'laravel-api'.
4. Continue to type 'cd laravel-api'
5. And last, type 'php artisan serve', then click on the URL shown in the terminal<br>
If it shows the Laravel web page, you're all set.<br>

##### Create Database and Migration
###### Create Database via HeidiSQL Laragon
On Laragon, click 'Database', which will automatically opens the HeidiSQL, and do the following:<br>
1. on the left-bottom side of HeidiSQL, click 'new'
2. give the 'unnamed' to 'yourName_db'.
3. Makesure your network type is MariaDB or MySQL (TCP/IP), Host 127.0.0.1, user=root, password _(left it empty if there's no password you've set)_, port=3306 _(by default most devs use 3306)_.
4. Click 'Open', it'll open another HeidiSQL Pop-Up.
5. On this new pop-up, right on the left-side of the menu, right-click the 'yourName_db' root > Create New > Database
6. Name: 'db_api_laravel', Collation: 'utf8mb4_0900_ai_ci' _(leave it default)_.<br><br>


### SantriKoding Laravel #2 - Create Model and Migration: 
Text-based Tutorial Link: [Tutorial RESTFUL API laravel 11 #2: Create Model and Migration _(Tutorial RESTFUL API laravel 11 #2: Membuat Model dan Migration)_](https://santrikoding.com/tutorial-restful-api-laravel-11-2-membuat-model-dan-migration) <br>
Video-based Tutorial Link: [Tutorial Restful API Laravel 11 #3 : Create Model and Migration _(Tutorial Restful API Laravel 11 #3 : Membuat Model dan Migration)_](https://www.youtube.com/watch?v=yYKGkmaPyG0&list=PL-2rLYVN9WCw34_TXFwl84r7DW9vwnj5s&index=3)<br>
**Please be advice:** This tutorial are spoken in Indonesian language.  For Simplicity, I'll guide you using simple English Language.<br>

**Branch: 'part1_modelAndMigration'**<br>

###### Configure the .env to connect with the DB
Go to the .env, and make some changes here:<br>
```
#DB_CONNECTION=sqlite<br>
DB_CONNECTION=mysql<br>
DB_HOST=127.0.0.1<br>
DB_PORT=3306<br>
DB_DATABASE=db_api_laravel<br>
DB_USERNAME=root<br>
DB_PASSWORD=<br>
```
First, laravel's DB_CONNECTION is sqlite by default, so give comment using hash '#' and create DB_CONNECTION to mysql. For the DB_PASSWORD, Leave the password empty by default.

###### Create the Model & Migration
In the VSCode terminal, type in:
```
php artisan make:model Post -m
```
This will automatically create the Post Model located in:<br>
- app/Models/Post.php _which is the model_, and
- XXXXX_create_posts_table.php *which is a Post Migration that'll be used to create new table instantly located in database/migrations/XXXX_create_posts_table.php.*<br>
On the Post Model, add protected fillable that contains 2 columns, which are 'title' and 'content' columns.
<br><br>
On the Post Migration in the up function, add the 'title' with string data type, and 'content' text data type.  In my own version, I add the 'idPosts' in the id data type, where it's more helpful for intermediate devs like myself.  For begineers, I'll suggest leave the id default (empty).  Because I like to challenge myself, I'll be creating the idPosts primary key, and on the model Post add the "protected $primaryKey = 'idPosts';".

###### Create the new Table using Migration
On the vscode terminal, type:
```
php artisan migrate
```
After that, hit the enter, and it will generate the new tables contained in the database/migrations directory.<br><br>

You can then go to the HeidiSQL page, click the refresh button on the top-left menu, and you'll notice there's updated new table in the 'yourName_db/db_api_laravel' on the left-side menu bar.<br>

### SantriKoding Laravel #3 - Create API Resources
Text-based Tutorial Link: [Tutorial Restful API Laravel 11 #3 : Create API Resources _(Tutorial Restful API Laravel 11 #3 : Creating API Resources)_](https://santrikoding.com/tutorial-restful-api-laravel-11-3-membuat-api-resources) <br>
Video-based Tutorial Link: [Tutorial Restful API Laravel 11 #4 : Create API Resources _(Tutorial Restful API Laravel 11 #4 : Membuat API Resources)_](https://www.youtube.com/watch?v=iWkmzcSI4L8&list=PL-2rLYVN9WCw34_TXFwl84r7DW9vwnj5s&index=4)<br>
**Please be advice:** This tutorial are spoken in Indonesian language.  For Simplicity, I'll guide you using simple English Language.<br>

**Branch: 'part2_createApiRes'**<br>

In this branch we're only adding the resources directory, with PostResource class in it, and make some modifications on the method by adding a public var declaration and a construct.<br>

Before I proceed into this Create API Resources course, I first went deep into this Laravel Docs that teaches the importance of using Eloquent Resources, and an overview of its concepts:<br>
- [Eloquent Resources](https://laravel.com/docs/11.x/eloquent-resources)<br>

#### Onto the practice
Create the resource directory and add class PostResource in the resource using this command in the VSCode Terminal:
```
php artisan make:resource PostResource
```
This will create a new file & directory in app/Http/Resources/PostResource.php<br>

You will have a new page that looks like this:<br>
```
<?php

namespace App\Http\Resources;

use Illuminate\Http\Request;
use Illuminate\Http\Resources\Json\JsonResource;

class PostResource extends JsonResource
{
    /**
     * Transform the resource into an array.
     *
     * @return array<string, mixed>
     */
    public function toArray(Request $request): array
    {
        return parent::toArray($request);
    }
}
```
Modify the PostResource.php by first defining 3 property variables which are $status, $message, $resource, that are essential to be use as an API:
```
<?php

namespace App\Http\Resources;

use Illuminate\Http\Request;
use Illuminate\Http\Resources\Json\JsonResource;

class PostResource extends JsonResource
{
    //define property
    public $status;
    public $message;
    public $resource;
    ...
```
After finish defining the property like above, next is to add construct method:
```
<?php
    ...
    /**
     * __construct
     *
     * @param  mixed $status
     * @param  mixed $message
     * @param  mixed $resource
     * @return void
     */
    public function __construct($status, $message, $resource)
    {
        parent::__construct($resource);
        $this->status  = $status;
        $this->message = $message;
    }
    ...
```
And on the toArray default method from laravel resource, change _return parent::toArray($request);_ into this:
```
<?php
    ...
    public function toArray(Request $request): array {
        return [
            'success' => $this->status,
            'message' => $this->message,
            'data'    => $this->resource
        ];
    }
```
#### Final Result
This will be the result of the app/Http/Resources/PostResource.php:
```
<?php

namespace App\Http\Resources;

use Illuminate\Http\Request;
use Illuminate\Http\Resources\Json\JsonResource;

class PostResource extends JsonResource
{
    // define property
    public $status;
    public $message;
    public $resource;
    /**
     * __construct
     * 
     * @param mixed $status
     * @param mixed $message
     * @param mixed $resource
     * 
     * @return void
     */
    public function __construct($status, $message, $resource) {
        parent::__construct($resource);
        $this->status = $status;
        $this->message = $message;
    }

    /**
     * Transform the resource into an array.
     * @param mixed $request
     * @return array<string, mixed>
     */
    public function toArray(Request $request): array
    {
        return [
            'success'   =>  $this->status,
            'message'   =>  $this->message,
            'data'      =>  $this->resource
        ];
    }
}

```
##### Conclussion
This branch part2_createApiRes that stands for 'Create API Resource Part 2' only shows on how to create Resource directory in the app/Http/Resources, before moving on to the next branch, that shows how to show data from database into the JSON format on branch part3_dbToJSON.<br><br>


<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
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

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[WebReinvent](https://webreinvent.com/)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Jump24](https://jump24.co.uk)**
- **[Redberry](https://redberry.international/laravel/)**
- **[Active Logic](https://activelogic.com)**
- **[byte5](https://byte5.de)**
- **[OP.GG](https://op.gg)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
