# Overleaf Toolkit with Review
This repository forked from Overleaf Toolkit and reference grandduke1106's add [review and comment](https://github.com/GrandDuke1106/sharelatex/tree/main) version

## How to start 
1. clone this repository
2. build sharelatex image like this
```sh
docker build . -t sharelatex/sharelatex:latest-with-review 
```
  - if u change the image name then update lib/docker-compose.base.yml sharelatex-image
```docker
services:
    sharelatex:
        restart: always
        image: sharelatex_image_name:tag <- update this part
        container_name: sharelatex
        ...
```
3. run `bin/up -d` and checking the app

more information check here : [Overleaf Toolkit](https://github.com/overleaf/toolkit)
