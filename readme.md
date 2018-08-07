### Queue killer
Kills all temp queues with 0 consumers on specific rabbitmq virtual host.  

#### Requirements
 - python 2.7
 - [rabbitmqadmin](https://www.rabbitmq.com/management-cli.html)
 
#### Install rabbitmqadmin
In commad replace {hostname} with domain name of sever with rabbitmq with rabbitmq_management plugin enabled
```shell
$ wget http://{hostname}:15672/cli/rabbitmqadmin
$ chmod ug+x rabbitmqadmin;
$ sudo mv ./rabbitmqadmin /usr/bin/;
```

#### Install script
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
$ sudo queue_killer VIRTUAL_HOST [USERNAME] [PASSWORD];
```
VIRTUAL_HOST - name of rabbitmq virtual host  
USERNAME - username with "administrator" access, default value "guest"  
PASSWORD - password, default value "guest"  
