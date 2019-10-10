# linux software installation
1. mongodb 27017
    ```shell
    $ sudo apt-get install mongodb 
    $ sudo service mongodb start/stop/restart
    # enter mongo cmd
    $ mongo
    m> use admin
    m> db.a
    # check port
    > netstat -ano | findstr 27017
    ```

2. mysql 3306 root:root
    ```shell
    $ sudo apt-get install mysql-server    
    $ sudo service mysql start/stop/restart
    $ sudo mysql-secure_installation
    $ sudo service mysql restart
    $ sudo mysql -uroot -p
    m> use mysql;
    m> update user set host = '%' where user = 'root';
    m> grant all privileges on *.* to 'root'@'%' identified by 'root';
    m> flush privileges;
    ```

3. redis 6379
    ```shell
    $ sudo apt-get install redis-server
    $ redis-server
    # cmd client
    $ redis-cli
    ```

4. rabbitmq 5672
    ```shell
    $ sudo apt-get install erlang-nox
    $ sudo apt-get install rabbitmq-server
    $ sudo service rabbitmq-server start/stop/restart
    $ sudo rabbitmqctl status
    # add user
    $ sudo rabbitmqctl add_user root root
    $ sudo rabbitmqctl set_user_tags root administrator
    $ sudo rabbitmqctl set_permissions -p / root '.*' '.*' '.*'
    # http://192.168.x.xx:15672
    ```