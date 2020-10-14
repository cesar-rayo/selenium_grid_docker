# Required images

```
$ docker images
REPOSITORY                    TAG                 IMAGE ID            CREATED             SIZE
selenium/node-firefox-debug   latest              da0a2ea98cb7        3 days ago          891MB
selenium/node-chrome-debug    latest              f6a0465fc69f        3 days ago          952MB
selenium/node-firefox         latest              88248990dbc4        3 days ago          859MB
selenium/node-chrome          latest              548ffd8b6b82        3 days ago          921MB
selenium/hub                  latest              e2cd04f4ddd3        3 days ago          264MB
```

```
$ sudo docker-compose up -d
Creating selenium_grid_docker_selenium-hub_1 ... done
Creating selenium_grid_docker_firefox_1      ... done
Creating selenium_grid_docker_chrome_1       ... done
```

This will start the grid at http://localhost:4444/grid/console

Common commands
```
$ docker-compose restart
$ docker-compose down
$ docker-compose up -d --scale chrome=10
```