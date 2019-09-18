# ACCENT test repository

## Installation

Clone both this repository and ACCENT's in the same directory:
```
cd MY_WORK_DIRECTORY
git clone git@github.com:theodo/accent.git
git clone git@github.com:theodo/accent_test.git
```

Go into this repository and start the Docker containers:
```
cd accent_test
docker-compose up -d
```

Install the Symfony project
```
docker-compose exec php composer install
```

## Check ACCENT

```
docker-compose exec php bin/console forge:access-control
```
