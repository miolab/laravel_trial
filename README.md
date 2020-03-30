# Laravel Mock

<img width="600" alt="laravel_trial" src="https://user-images.githubusercontent.com/33124627/77863897-b1954c80-7260-11ea-8a92-040b9811b737.png">

---

## Usage

```
$ git clone https://github.com/miolab/laravel_trial.git

$ cd laravel_trial

$ docker-compose up -d --build

$ docker-compose exec app ash

/work # composer install

/work # cp .env.example .env

/work # php artisan key:generate

/work # php artisan migrate

```

[http://127.0.0.1:10080/](http://127.0.0.1:10080/) で確認

* `$ ...` はTerminalでの操作。

* `/work # ...` はDockerコンテナ内での操作。

* コンテナやイメージをまとめて全削除

  ```
  $ docker-compose down --rmi all --volumes
  ```

---

## 実行環境

| | バージョン |
|:--|:--|
| Mac | |
| Docker | 19.03.8 |
| Docker-compose | 1.25.4 |
| PHP | 7.3.16 |
| Composer | 1.10.1 |
| Laravel Framework | 6.18.3 |
| Nginx | 1.17.9 |
| MySQL | 8.0.19 |


## ディレクトリ構成

```
$ tree -L 3 .
.
├── README.md
├── docker
│   ├── mysql
│   │   └── my.cnf
│   ├── nginx
│   │   └── default.conf
│   └── php
│       ├── Dockerfile
│       └── php.ini
├── docker-compose.yml
├── logs
│   ├── access.log
│   ├── error.log
│   ├── mysql-error.log
│   ├── mysql-query.log
│   ├── mysql-slow.log
│   └── php-error.log
└── src
    ├── app
    │   ├── Console
    │   ├── Exceptions
    │   ├── Http
    │   ├── Providers
    │   └── User.php
    ├── artisan
    ├── bootstrap
    │   ├── app.php
    │   └── cache
    ├── composer.json
    ├── composer.lock
    ├── config
    │   ├── app.php
    │   ├── auth.php
    │   ├── broadcasting.php
    │   ├── cache.php
    │   ├── database.php
    │   ├── filesystems.php
    │   ├── hashing.php
    │   ├── logging.php
    │   ├── mail.php
    │   ├── queue.php
    │   ├── services.php
    │   ├── session.php
    │   └── view.php
    ├── database
    │   ├── factories
    │   ├── migrations
    │   └── seeds
    ├── package.json
    ├── phpunit.xml
    ├── public
    │   ├── favicon.ico
    │   ├── index.php
    │   ├── robots.txt
    │   └── web.config
    ├── readme.md
    ├── resources
    │   ├── js
    │   ├── lang
    │   ├── sass
    │   └── views
    ├── routes
    │   ├── api.php
    │   ├── channels.php
    │   ├── console.php
    │   └── web.php
    ├── server.php
    ├── storage
    │   ├── app
    │   ├── framework
    │   └── logs
    ├── tests
    │   ├── Bootstrap.php
    │   ├── CreatesApplication.php
    │   ├── Feature
    │   ├── TestCase.php
    │   └── Unit
    ├── vendor
    │   ├── autoload.php
    │   ├── bin
    │   ├── composer
    │   ├── dnoegel
    │   ├── doctrine
    │   ├── dragonmantank
    │   ├── egulias
    │   ├── facade
    │   ├── fideloper
    │   ├── filp
    │   ├── fzaninotto
    │   ├── hamcrest
    │   ├── jakub-onderka
    │   ├── laravel
    │   ├── league
    │   ├── mockery
    │   ├── monolog
    │   ├── myclabs
    │   ├── nesbot
    │   ├── nikic
    │   ├── nunomaduro
    │   ├── opis
    │   ├── paragonie
    │   ├── phar-io
    │   ├── phpdocumentor
    │   ├── phpoption
    │   ├── phpspec
    │   ├── phpunit
    │   ├── psr
    │   ├── psy
    │   ├── ramsey
    │   ├── scrivo
    │   ├── sebastian
    │   ├── swiftmailer
    │   ├── symfony
    │   ├── theseer
    │   ├── tijsverkoyen
    │   ├── vlucas
    │   └── webmozart
    └── webpack.mix.js
```
