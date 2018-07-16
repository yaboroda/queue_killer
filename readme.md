### Queue killer
Kills all temp queues with 0 consumers on specific rabbitmq virtual host.  

#### Requirements
 - python 2.7
 - [rabbitmqadmin](https://www.rabbitmq.com/management-cli.html)

#### Install
you can download script
```shell
$ wget https://raw.githubusercontent.com/yaboroda/queue_killer/master/queue_killer;
$ chmod ug+x queue_killer;
$ sudo mv ./queue_killer /usr/bin/;
```
or clone repo
```shell
$ git clone https://github.com/yaboroda/queue_killer;
$ cd queue_killer/;
$ sudo ln -s $(pwd)/queue_killer /usr/bin/queue_killer
```

#### Usage
```shell
$ sudo queue_killer VIRTUAL_HOST;
```
where VIRTUAL_HOST is name of rabbitmq virtual host
