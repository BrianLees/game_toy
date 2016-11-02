# gamify

To get a working container:

```docker-compose build```

```docker-compose up -d # The -d runs in detached mode```

```docker-compose run -d app rails db:create```

```docker-compose run -d app rails db:migrate```


To get a bash shell in the container: ```docker exec -it <mycontainer> bash```

Setup and run tests:
```docker-compose run -e "RAILS_ENV=test" app bin/rails db:create db:migrate```

```docker-compose run -e "RAILS_ENV=test" app bin/rails test```

#### Docker Container
The ["Running a Rails development environment in Docker"](http://blog.codeship.com/running-rails-development-environment-docker/) article was used to configure the first iteration of the Docker container.
