# php-caddy

[![Docker Build](https://github.com/dockhippie/php-caddy/actions/workflows/docker.yml/badge.svg)](https://github.com/dockhippie/php-caddy/actions/workflows/docker.yml) [![GitHub Repo](https://img.shields.io/badge/github-repo-yellowgreen)](https://github.com/dockhippie/php-caddy)

These are docker images for [PHP][upstream] running on our
[Caddy image][parent].

## Versions

For the available versions please look at [Docker Hub][dockerhub] or
[Quay][quayio] or check the existing folders within the
[GitHub repository][github].

## Volumes

*  /srv/www
*  /etc/php7/custom.d
*  /etc/php8/custom.d

## Ports

*  8080

## Available environment variables

```bash
PHP_COMPOSER_INSTALL = true
PHP_COMPOSER_ROOT = ${CADDY_WEBROOT}
PHP_DATE_TIMEZONE = UTC
PHP_DISPLAY_ERRORS = On
PHP_DISPLAY_STARTUP_ERRORS = On
PHP_ERROR_LOG = /proc/self/fd/2
PHP_ERROR_REPORTING = E_ALL & ~E_DEPRECATED & ~E_STRICT
PHP_HTML_ERRORS = On
PHP_IGNORE_REPEATED_ERRORS = Off
PHP_IGNORE_REPEATED_SOURCE = Off
PHP_LOG_ERRORS = On
PHP_LOG_ERRORS_MAX_LEN = 1024
PHP_LOG_LEVEL = warning
PHP_MAX_CHILDREN = 75
PHP_MAX_EXECUTION_TIME = 3600
PHP_MAX_INPUT_TIME = 3600
PHP_MAX_REQUESTS = 500
PHP_MEMORY_LIMIT = 512M
PHP_POST_MAX_SIZE = 2G
PHP_PROCESS_IDLE_TIMEOUT = 10s
PHP_REPORT_MEMLEAKS = On
PHP_TRACK_ERRORS = Off
PHP_UPLOAD_MAX_FILESIZE = 2G
```

## Inherited environment variables

*  [webhippie/caddy](https://github.com/dockhippie/caddy#available-environment-variables)
*  [webhippie/alpine](https://github.com/dockhippie/alpine#available-environment-variables)

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

*  [Thomas Boerger](https://github.com/tboerger)

## License

MIT

## Copyright

```console
Copyright (c) 2015 Thomas Boerger <http://www.webhippie.de>
```

[upstream]: https://secure.php.net
[parent]: https://github.com/dockhippie/caddy
[dockerhub]: https://hub.docker.com/r/webhippie/php-caddy/tags
[quayio]: https://quay.io/repository/webhippie/php-caddy?tab=tags
[github]: https://github.com/dockhippie/php-caddy
