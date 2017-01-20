# FASHION SENSE

## Description

## Install
* [install Docker](https://docs.docker.com/engine/installation/)
* [install Docker Compose](https://docs.docker.com/compose/install/)

## Usage

* check out [this](https://git-scm.com/book/en/v2/Git-Tools-Submodules) page to learn about git submodules

* basically what you want to do is run this command to get everything
```
$ git clone --recursive https://github.com/sgp715/FashionSense.git
```
* then build it with Docker Compose
```
$ docker-compose build
```

* then run it with Docker Compose
```
$ docker-compose up
```
* if you want to update from the submodules you need to follow these steps

    * first cd into that submodule directory
    * next checkout a branch
    ```
    $ git checkout [branch]
    ```
    * and set yourself to update remotes
    ```
    $ git submodule update --remote --merge
    ```
* if you simply are behind and want to update your module, go inside the submodule and run
```
$ git fetch
$ git merge [repo/branch]
```
* to update all submodules to point to most recent
```
$ git submodule foreach git pull origin master
```
