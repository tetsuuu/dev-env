# Create develop environment by Docker
Create environment for develop on local.

Run following command in your terminals.<br>
&emsp;&emsp;`docker-compose up -d`


# Nginx container
This is basically Dockerfile from official repository.<br>
Volume mounted form `nginx` && `www/html` for config and index.<br>
You can access to *http://localhost:80* default.
If you wanna change URL, should be change `nginx/nginx.conf` by yourself please.

# PHP container
Pull official image `php:7.2-fpm` and injection `ini`file.<br>

# MySQL DB container
It's pulled by official.<br>
Default mountpoint is `mysql/date` in this directory.<br>
If you wanna change that refactor *volume* section on `docker-compose.yml`

# MySQL GUI container
*phpMyAdmin* is MySQL GUI tools.<br>
Maybe you don't need, should be commentout.
 


