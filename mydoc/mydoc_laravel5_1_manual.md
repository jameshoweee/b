---
title: laravel5-1
tags: [getting_started]
keywords: release notes, announcements, what's new, new features
last_updated: March 20, 2016
summary: "laravel 5-1"
sidebar: mydoc_sidebar
permalink: /mydoc_laravel5_1_manual/
---


## a 文档资料

[官方文档](https://laravel.com/docs/5.1)

[laravel学院 发行版本说明 差异对比](http://laravelacademy.org/post/9.html)

新建指定版本项目:

	composer create-project laravel/laravel blog "5.1.*"

[laravel.com 5.1](https://laravel.com/docs/5.1/seeding)

[laravelbook Migrations](http://laravelbook.com/laravel-migrations-managing-databases/)

### 环境设置

	subl 	~/.homestead-56/Homestead.yaml

## 常用操作

	php artisan migrate
	php artisan db:seed
	composer install
	composer update

	php artisan vendor:publish			生成配置文件

####  [sitepoint migrations](http://www.sitepoint.com/laravel-migrations/)

## laravel5.1



#### ryanchenkie

ONE [Token-Based Authentication for AngularJS and Laravel Apps ](https://scotch.io/tutorials/token-based-authentication-for-angularjs-and-laravel-apps) 5.1

TWO Authenticated User Route [Token-Based Authentication for AngularJS and Laravel Apps](http://ryanchenkie.com/token-based-authentication-for-angularjs-and-laravel-apps/)

#### huanghua581

[dingo-api-demo](https://github.com/huanghua581/dingo-api-demo)

jwt-auth 、短信

github中搜 dingo

### Laravel-5-Bootstrap-3-Starter-Site
[Laravel-5-Bootstrap-3-Starter-Site](https://github.com/mrakodol/Laravel-5-Bootstrap-3-Starter-Site/issues/205)

项目启动的步骤:

	$ composer dump-autoload
	$ composer install --no-scripts
	$ npm install --save-dev
	$ gulp
	$ php artisan migrate
	$ php artisan db:seed
	$ php artisan key:generate			//重要
	👍 3  
	
#### laravel视频

[基础教程](https://laravist.com/series/laravel-5-basic)

[稍微深入](https://laravist.com/series/dive-a-little-deep-into-laravel-5)

#### tool_jwt

[tool_jwt_](http://kjur.github.io/jsjws/tool_jwt.html)

## 例子

[l.njbccw.cn](http://l.njbccw.cn/tasks)

### laravel-api-boilerplate-jwt

    artisan api:route
    
### java jwt-token

   [java jwt token atlassian](https://developer.atlassian.com/static/connect/docs/latest/concepts/understanding-jwt.html)