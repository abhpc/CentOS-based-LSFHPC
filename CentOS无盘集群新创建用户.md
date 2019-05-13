以下例子为创建一个用户名为"james"的用户

#### 1. root用户执行以下命令，指定其home目录

    # useradd james -d /home/james

#### 2. 为james用户设置密码，注意Linux下输入密码不会有任何显示，根据提示，重复输入密码即可。

    # passwd james

#### 3. root告知集群其他节点：

    # make -C  /var/yp

#### 4. 为james用户初始化：

    # su james
    $ cd
    $ initialize.sh

连续回车后，初始化完成。
