## php-nginx-composer

This is a Dockerfile/image to build a container for nginx, php7.2-fpm and composer.

### Features

- You can use git to pull and push code within the container,
- You can create and edit files using nano.
- You can use Supervisor for configuring multiple sites.
- You can use Cron, ssl, unzip.

## PHP Extensions/Modules

```
    [PHP Modules]
    calendar
    Core
    ctype
    curl
    date
    dom
    exif
    fileinfo
    filter
    ftp
    gd
    gettext
    hash
    iconv
    intl
    json
    ldap
    libxml
    mbstring
    mcrypt
    memcache
    mysqli
    mysqlnd
    odbc
    openssl
    pcntl
    pcre
    PDO
    pdo_dblib
    pdo_mysql
    PDO_ODBC
    pdo_pgsql
    pdo_sqlite
    pgsql
    Phar
    posix
    readline
    Reflection
    session
    shmop
    SimpleXML
    soap
    sockets
    sodium
    SPL
    sqlite3
    standard
    sysvmsg
    sysvsem
    sysvshm
    tidy
    tokenizer
    wddx
    xml
    xmlreader
    xmlrpc
    xmlwriter
    xsl
    Zend OPcache
    zip
    zlib

    [Zend Modules]
    Zend OPcache
```
Nginx uses `php-fpm`for processing php requests through FastCGI.

Ports 80, 3306 and 22 are exposed.

Composer is installed globally for use.

## Get Started

To pull from Docker Hub-

```shell
    docker pull ankitjain28/php-nginx-composer:latest
```

## Running containers

To run a container -

```shell
    sudo docker run --name <container-name> -d ankitjain28/php-nginx-composer
```

To run commands within Container -

```shell
    sudo docker exec -it <container-name> <commands>
```

Stop the Container -

```shell
    sudo docker stop <container-name>
```

Start the Container -

```shell
    sudo docker start <container-name>
```

Delete the Container -

```shell
    sudo docker rm <container-name> -f
```
