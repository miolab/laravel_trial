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

[http://127.0.0.1:10080/](http://127.0.0.1:10080/)

* `$ ...` はTerminalでの操作。

* `/work # ...` はDockerコンテナ内での操作。


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
