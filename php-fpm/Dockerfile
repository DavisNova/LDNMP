# 使用官方 PHP-FPM 镜像作为基础
FROM php:7.4-fpm

# 安装 mysqli 扩展和其他必要的扩展
RUN apt-get update && apt-get install -y libpng-dev libjpeg-dev libfreetype6-dev && docker-php-ext-install gd mysqli pdo pdo_mysql

# 启用 mysqli
RUN docker-php-ext-enable mysqli
