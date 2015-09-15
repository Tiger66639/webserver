# webserver

[![Build Status](https://travis-ci.org/Tiger66639/webserver.svg)](https://travis-ci.org/Tiger66639/webserver)
# Introduction

Are you serious? A web server written in pure PHP for PHP? Ohhhh Yes! :) This is a HTTP/1.1 compliant webserver written in php.
And the best... it has a php module and it's multithreaded!

We use this in the [`appserver.io`](<http://www.appserver.io>) project as a server component for handling HTTP requests.

# Installation

If you want to use the web server with your application add this

```sh
{
    "require": {
        "appserver-io/webserver": "dev-master"
    },
}
```

to your ```composer.json``` and invoke ```composer update``` in your project.

# Usage

If you can satisfy the requirements it is very simple to use the webserver. Just do this:
```bash
git clone https://github.com/Tiger66639/webserver
cd webserver
PHP_BIN=/path/to/your/threadsafe/php-binary bin/webserver
```

If you're using [`appserver.io`](<http://www.appserver.io>) the start line will be:
```bash
bin/webserver
```

Goto http://127.0.0.1:9080 and if all went good, you will see the welcome page of the php webserver.
It will startup on insecure http port 9080 and secure https port 9443.

To test a php script just goto http://127.0.0.1:9080/info.php and see what happens... ;)

# Semantic versioning

This library follows semantic versioning and its public API defines as follows:

* The public API, configuration and entirety of its modules
* The public interface of the `\AppserverIo\WebServer\ConnectionHandlers\HttpConnectionHandler` class
* The public interfaces within the `\AppserverIo\WebServer\Interfaces` namespace

# External Links

* Documentation at [appserver.io](http://docs.appserver.io)
