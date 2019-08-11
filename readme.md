Based on the Udemy Course by Edwin Diaz:

<a href="https://www.udemy.com/php-with-laravel-for-beginners-become-a-master-in-laravel/">PHP with Laravel for beginners - Become a Master in Laravel</a>


Common Commands:


Step 1a: Open the console and cd to root directory of your project.

Step 1b: Create a .env file in your root directory <a href=".env.example">based on this</a>

Step 1c: Create a MySQL instance - maybe with xampp, and add the creds to your new .env file.

Step 2: Run ```composer install``` or php composer.phar install.

Step 3: Run 

```
php artisan key:generate
```

This command will log something like this:

```
Application key [base64:8onaHu6KVgdsgsdgsdgyROBZBZnNrj1L/tbuQmOvhCdk=] set successfully.
```

Copy-paste that base64... into your .env file, to a var called "APP_KEY"


Step 4: Run ```php artisan migrate```

Step 5: Run ```php artisan db:seed``` run seeders, if any.

Step 6: Run ```php artisan serve```


<h1>Trouble-Shooting</h1>

Something not working correctly? 

a) Run the phpinfo() command, or start xampp and browse to

http://localhost/dashboard/phpinfo.php

b) Check out:

https://bobcares.com/blog/laravel-something-went-wrong/

c) Running xampp on linux:

```
sudo /opt/lampp/lampp start
```

```
sudo /opt/lampp/lampp stop
```

```
sudo /opt/lampp/lampp restart
```


<h1>Prerequisites</h1>

You have a MySQL host to connect to. Try Xampp, for example.
