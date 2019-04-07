This project uses [My Anime List](https://www.kaggle.com/azathoth42/myanimelist/version/9) data to investigate the effect of caching in reducing the pressure to the database.

## Set up Docker Database Image
1. Download the [My Anime List](https://www.kaggle.com/azathoth42/myanimelist/version/9) csv file
1. `docker pull postgres`
1. `docker run --name cacheDB -p 9999:5432 -d postgres:latest` 
1. Check the connection on `postgres@localhost:9999/postgres` 
1. Import the csv file to the docker container
