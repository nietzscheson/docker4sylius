Docker environment for Sylius Project
============

Installation
============

Step 1: Clone docker4sylius repository
---------------------------

```console
$ git clone git@github.com:nietzscheson/docker4sylius.git
```

Step 2: Clone Sylius-Standard repository
-------------------------

```console
$ git clone git@github.com:Sylius/Sylius-Standard.git sylius
```

Step 3: Install Sylius vendors
-------------------------

```console
$ docker-compose run --rm php composer install
```

Step 4: Install Sylius
-------------------------

```console
$ docker-compose run --rm php bin/console sylius:install
```

Step 5: Install and build assets vendors
-------------------------
```console
$ docker-compose run --rm node yarn install

$ docker-compose run --rm node yarn install
```

That's all. Try and fun!!!

-----------

License
-------

This bundle is published under the [MIT License](LICENSE)

