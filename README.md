![alt text](http://halusanation.com/wp-content/uploads/2014/12/php_skeleton_app.jpg "The PHP Skeleton App Header Image")

# The PHP Skeleton App

The PHP Skeleton App creates an object-oriented PHP MVC environment, tailored for rapid development. The environment makes use of the [Slim PHP micro framework](http://slimframework.com/), [Twig](http://twig.sensiolabs.org/) for templating, and [Twitter Bootstrap 3](http://getbootstrap.com/) for the theme.

Out of the box, it provides the ability to set up and run a public-facing website, authenticate to the administrative side, and create users and groups. All of the baseline database tables are created on first run, along with the first "Universal Administrator".

**Note: The PHP Skeleton App is currently under development and perpetually evolving.**

This is my first go at publishing something extensive on GitHub. I'm far from perfect, and have been in somewhat of a bubble. Regardless, I have decided to get my feet wet so I can collect feedback from the community, and grow as a developer. So, your constructive criticism is encouraged. I'll do my best to learn from my mistakes and deliver the goods.

Thanks!

-Gor

* * *

## Features

* **Quick 5-minute installation**

* **Simple configuration**

* **Easy templating with custom views using Twig**

* **Twitter Bootstrap 3.3.x**

    "Carousel" template included for the public website

    "Dashboard" template included for the administrative interface

* **Site Module**

    The public site

* **Authenticate Module**

    With local authentication, out-of-the-box. Oauth schemes coming soon (e.g. Twitter, Google, Facebook, Github).

* **User Account Module**

    For user management, complete with a self-registration form and the ability to reset forgotten passwords.

* **Group Module**

    Assign users to groups for greater control over permissions

* **Dashboard Module**

    Default landing page for the administrative side

* **More coming soon...**

* * *

## Requirements (LAMP)

*These requirements are what I have found to be true. It's likely that I may have missed something along the way. If so, please let me know.*

##### Linux
* So far, only tested on Linux Ubuntu 14.04 (trusty)

##### Apache
* Modules: alias, deflate, dir, env, headers, mime, php5, rewrite, setenvif

##### MySQL

##### PHP >= 5.3
* Extensions: FileInfo, mysql, PDO, pdo_mysql, php5-curl, php5-json, php5-mcrypt

##### Git

##### Composer

#### Environment Check

To check to see if you have all of the necessary components in place, you can run the "Environment Check" script:

```bash
http://YOUR_DOMAIN/webapp_installer/library/env.php
```

* * *

## Getting Started

### STEP 1

#### Run Composer (non global installation)

```bash
php composer.phar create-project ghalusa/php-skeleton-app /PATH/TO/YOUR_EMPTY_WEB_ROOT_DIRECTORY/ dev-master
```

#### OR... Run Composer (global installation)

```bash
composer create-project ghalusa/php-skeleton-app /PATH/TO/YOUR_EMPTY_WEB_ROOT_DIRECTORY/ dev-master
```

### STEP 2

#### First, Make Sure Apache Has Permissions to Do Stuff
*(This can be changed back after the installation is finished.)*

```bash
sudo chown -R www-data:www-data /PATH/TO/YOUR_EMPTY_WEB_ROOT_DIRECTORY/
```

### STEP 3

#### Run the Web App Installer...

##### Point your browser to the root of your web environment...

```bash
http://YOUR_DOMAIN/
```

##### ... And Fill Out the Form

You will need:

* A valid email address for the creation of the administrative account.
* The location, username, and password of a MySQL database.

#### That's It!

At this point, you should have successfully spawned a complete "PHP Skeleton App". Dig in, and start adding your own "Modules"!

* * *

## Documentation

* [PHP Skeleton App Documentation](http://phpskeleton.com/) (coming soon)
* [PHPDocs](http://phpskeleton.com/docs/)
* Until I get the documentation out there, you can look at the anatomy of any of the modules which are included and present by default.
* On deck: I'm going to develop a "Module Creator", which will spawn a bare-bones module at the click of a button, or via command line.

## About the Author

The PHP Skeleton App is created and maintained by [Goran Halusa](http://halusanation.com/), a Web Architect, artist, musician, and chef.

### Twitter

Follow [@goranhalusa](http://www.twitter.com/goranhalusa) on Twitter to receive the very latest news and updates about The PHP Skeleton App.

### Acknowledgements

* [PHP Weekly](http://phpweekly.com/): Thanks for including The PHP Skeleton App in your [weekly email](http://www.phpweekly.com/archive/2015-01-01.html)!

### Disclaimer

The PHP Skeleton App is in active development, and test coverage is continually improving.

* * *

## Open Source License

The PHP Skeleton App is released under the MIT public license.
