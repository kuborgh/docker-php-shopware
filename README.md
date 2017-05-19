# docker-php-shopware
Docker PHP-FPM Container for shopware projects. It is configured with following PHP extensions
* bz2
* dom 
* exif
* fileinfo
* hash
* iconv
* mcrypt
* intl
* opcache
* pcntl
* pdo
* pdo_mysql
* pdo_sqlite
* readline
* session
* simplexml
* xml
* xsl
* zip
* gd
* APCu
* ioncube loader

The `xdebug` variant has xdebug installed and enabled. It should only be used on non-production environments!

## Mailing
NOTE: To enable mailing, you need to configure ssmtp. This can be done by adding a file `ADD ssmtp.conf /etc/ssmtp/` containing a config like this
```
# See https://linux.die.net/man/5/ssmtp.conf
Mailhub=<Server>
AuthUser=<User>
AuthPass=<Pass>
Hostname=<Senders Host>
FromLineOverride=YES
UseTLS=YES
UseSTARTTLS=YES
```
