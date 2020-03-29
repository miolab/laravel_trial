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

* `$ ...` はTerminalでの操作。

* `/work # ...` はDockerコンテナ内での操作。

