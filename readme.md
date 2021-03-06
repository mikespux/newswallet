# News Wallet

## Client Problem Statement 

I read a lot of news articles and many are the times I find very good articles that are worth saving for future reference. As it stands, there is no better way to do this other than bookmark the link to the site on my browser or save it on Opera Mini, options that I don’t find helpful for my needs.


## Getting started

*(Assuming you've [installed Laravel](https://laravel.com/docs/5.7/installation))*

Fork this repository, then clone your fork, and run this in your newly created directory:

``` bash
composer install
```

Next you need to make a copy of the `.env.example` file and rename it to `.env` inside your project root.

Run the following command to generate your app key:

```
php artisan key:generate
```

Update database credentials on the ```.env``` and run the command:
```
php artisan migrate --seed
```
Then start your server:

```
php artisan serve
```


Your Laravel starter project is now up and running! 


Check the ```PostmanCollection.json``` file to see the available APIs. 

For more APIs, open your browser and type:
```
http://localhost:8000/docs
```

## Deploying your Laravel application

Once you've created your website, an easy way to deploy your Laravel application is to use [Heroku](http://www.heroku.com). Just follow these few simple steps once you have successfully [signed up](https://id.heroku.com/signup/www-header) and [installed the Heroku toolbelt](https://toolbelt.heroku.com/):

Create a new Heroku application

```
$ heroku create
```

Initialize a new Git repository:

```
$ git init
$ heroku git:remote -a your-heroku-app-name
```

Commit your code to the Git repository if you haven't already:

```
$ git add .
$ git commit -am "make it better"
```

Set a Laravel encryption key:

```
$ heroku config:set APP_KEY=$(php artisan --no-ansi key:generate --show)
```

Push to Heroku:

```
$ git push heroku master
```

You can now browse your application online:

```
$ heroku open
```

You can read more about launching your project with Heroku here in their [Laravel & Heroku guide](https://devcenter.heroku.com/articles/getting-started-with-laravel).

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
