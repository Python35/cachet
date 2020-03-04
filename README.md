

1.  Clone this repo

2. Clone the official repo of CachetHQ/Cachet here and do composer install:

  ```shell
  git clone https://github.com/CachetHQ/Cachet.git
  ```
3. Replace PgSqlRepository.php file in Cachet/app/Repositories/metric with the file present in this repo.

4. Setup the Cachet project:

Note: This requires [Composer](https://getcomposer.org/) be installed on your Docker host.  

 ```shell
cd Cachet
composer install
cp ../conf/.env.docker ./.env
cd ..
```

5. Add APP KEY in Dockerfile Line 10.

6. Build the container:

  ```shell
  docker build -t cachet .
  ```
