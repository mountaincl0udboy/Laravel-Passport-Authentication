<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Getting started

## Installation

Please check the official laravel installation guide for server requirements before you start. [Official Documentation](https://laravel.com/)

Clone the repository

    git clone https://github.com/ogkkk/Laravel-Passport-Authentication.git

Switch to the repo folder

    cd Laravel-Passport-Authentication

Install all the dependencies using composer

    composer install

Copy the example env file and make the required configuration changes in the .env file

    cp .env.example .env

Generate a new application key

    php artisan key:generate

Run the database migrations (**Set the database connection in .env before migrating**)

    php artisan migrate

Start the local development server

    php artisan serve

You can now access the server at http://localhost:8000

**TL;DR command list**

    git clone https://github.com/ogkkk/Laravel-Passport-Authentication.git
    cd Laravel-Passport-Authentication
    composer install
    cp .env.example .env
    php artisan key:generate
    
**Make sure you set the correct database connection information before running the migrations** [Environment variables](#environment-variables)

    php artisan migrate
    php artisan serve
    
## Register API:
### You can test the Laravel Passport API for registering the user:
POST **http://localhost:8000/api/register**

![image](https://user-images.githubusercontent.com/85111590/204125968-51726901-b07c-4f34-9141-5b64f795660f.png)

## Login Passport API:
### After sign up, copy the Bearer token, set into the Headers section in the Postman app. Check out the Laravel Passport Endpoint for logging-in:
POST **http://localhost:8000/api/login**

![image](https://user-images.githubusercontent.com/85111590/204126272-f7353ef4-8691-4182-9b47-acae378a90a9.png)

## Passport Post Create API:
### To perform the CRUD operation, we need to set the correct authenticity. After successful registration and login, you will receive the access token. The manifestation of access token creates coherence with authorization, and It establishes secure communication with the server. You need to set this access token as a Bearer Token in the Authorization header.
POST **http://localhost:8000/api/posts**

![image](https://user-images.githubusercontent.com/85111590/204126388-087e16cb-b351-4e35-90a9-1f93087a762b.png)

## Post List API:
GET **http://localhost:8000/api/posts**

![image](https://user-images.githubusercontent.com/85111590/204126510-4b4a2b76-0acc-4a6e-8669-05671d258e05.png)

## Show Single Post API:
GET **http://localhost:8000/api/posts/{id}**

![image](https://user-images.githubusercontent.com/85111590/204126585-cf1c2470-0bee-4ba5-90db-4c5ba86c0434.png)

## Post Update API:
PUT **http://localhost:8000/api/posts/{id}**

![image](https://user-images.githubusercontent.com/85111590/204126667-54955a01-52cb-4c49-b2dd-4288af4bd29a.png)

## Post Delete API:
DELETE **http://localhost:8000/api/posts/{id}**

![image](https://user-images.githubusercontent.com/85111590/204126732-39b16343-7482-42af-977e-2d3e844b69d3.png)

Contact
If you have any questions about Laravel-Passport-Authentication, please feel free to contact.
