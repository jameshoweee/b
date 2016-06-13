---
title: task52-github
keywords: task52 github login
last_updated: March 20, 2016
tags: [getting_started]
summary: "task52 github login."
sidebar: mydoc_sidebar
permalink: /mydoc_about/
---

问题的提出:在完成了[带用户功能的任务管理系统](http://laravelacademy.org/post/3297.html#comments)之后追加[github登录功能](http://laravelacademy.org/post/1305.html)。


### 1、用户表追加了两个字段

[2016_06_01_070231_add_github_id_avatar_to_users](https://github.com/jnuc093/study_quickstart-intermediate/blob/master/database/migrations/2016_06_01_070231_add_github_id_avatar_to_users.php)

	php artisan migrate

### 2、路由定义


	php artisan make:controller SocialAuthController

在routes.php中添加:

	Route::get('auth/github', 'SocialAuthController@redirectToProvider');
	Route::get('auth/github/callback', 'SocialAuthController@handleProviderCallback');
	
> 在5.2.31	版本后 web middleware [为默认设置](https://github.com/laravel/laravel/commit/5c30c98db96459b4cc878d085490e4677b0b67ed)所以上定义的路由的方式基本与5.1一致

### 3、在resources/views/auth/login.blade.php登录按钮下添加:

	<a class="btn btn-link" href="auth/github">GitHub Login</a>

### 4、按照[github登录功能](http://laravelacademy.org/post/1305.html)设置自己的相应配置

  为了方便字体加载`resources/views/layouts/app.blade.php`文件中将
  
 	 https://fonts.googleapis.com/css替换为 https://fonts.useso.com/css
  
 

### 5、至此可以用自己github账号登录

所有实现的的代码在这 [study_quickstart-intermediate-github-login](https://github.com/jnuc093/study_quickstart-intermediate/)

### 6 添加DingoAPI JWT

RouteServiceProvider中添加 Http/api_routes.php文件并定义api

    artisan api:route

### 其他参考资料

[Matt Stauffer ](https://mattstauffer.co/blog/using-github-authentication-for-login-with-laravel-socialite)

