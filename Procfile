# web:  vendor/bin/heroku-php-nginx -C nginx.conf  -F fpm_custom.conf public/
web: heroku-php-apache2 public/ -C apache.conf
release: bin/console importmap:install && bin/console asset-map:compile && bin/console d:m:m -n --allow-no-migration
