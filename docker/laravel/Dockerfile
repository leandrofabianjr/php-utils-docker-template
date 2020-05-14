FROM composer

# Laravel installation
RUN composer global require laravel/installer
# Adding to path
RUN ln -s /tmp/vendor/bin/laravel /usr/sbin/laravel

ENTRYPOINT ["/usr/sbin/laravel"]
VOLUME /app
