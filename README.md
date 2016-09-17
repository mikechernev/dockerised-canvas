Docker setup for [Canvas](https://github.com/austintoddj/canvas) using PHP7-FPM and Nginx

## Instructions
1. Checkout the repository
* Run `cp .env.sample canvas/.env` 
* Run `docker run --rm -it -v $(pwd)/canvas:/code -w /code composer/composer install`
* Run `docker-compose up`
* Run `docker-compose run --rm php php /code/artisan canvas:install`
* Navigate to [http://localhost:8080](http://localhost:8080) in a browser
* See [Canvas instructions](https://github.com/austintoddj/canvas/blob/master/README.md) for more info
* Be a happy potato!

That's it! You have your local [Canvas](https://github.com/austintoddj/canvas) setup using Docker
  
 