# Docker quick start

Quick start for a PHP/MySQL local development web app using Docker.

## Setup

* Install Docker
* Clone and checkout this repo
* Set your ServerName in `.docker/vhost.conf` and your hosts file, for example `127.0.0.1 quickstart.local`
* Set your environment variables in `docker-compose.yml` - MySQL connection details etc.
* Create the `.docker/mysql/data` directory. 
* Run `docker-compose build` to build and then `docker-compose up` to start, you can do this in one go with `docker-compose up --build`
* Add your code to the `src` directory, you now have a working app using Docker.
* If you are using composer you can install dependencies by running `docker-compose exec app composer install` 

If you need additional php extensions, add them to `.docker/Dockerfile`, for anything else custom, the web is a great
resource.
