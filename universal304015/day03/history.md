# History
```shell
root@ip-172-31-2-188:~/dockerfile# history
    1  whoami
    2  ls
    3  cd /
    4  ls
    5  cd
    6  mkdir ~/work
    7  cd work/
    8  ls
    9  ssh-keygen
   10  cat ~/.ssh/id_rsa
   11  cat ~/.ssh/id_rsa.pub 
   12  git
   13  git clone https://github.com/weable-kosa/kosa-msa-2024-1st.git
   14  git@github.com:aj172019/practical-dev.github.io.git~
   15  git@github.com:aj172019/practical-dev.github.io.git
   16  git clone git@github.com:aj172019/practical-dev.github.io.git
   17  curl -fsSL https://get.docker.com -o install-docker.sh~
   18  curl -fsSL https://get.docker.com -o install-docker.sh
   19  ls
   20  
   21  cat install-docker.sh
   22  sh install-docker.sh --dry-run
   23  sudo sh install-docker.sh
   24  docker -v
   25  docker ps
   26  ls
   27  cd practical-dev.github.io/
   28  ls
   29  cd ..
   30  ls
   31  git clone git@github.com:aj172019/practical-dev.github.io.git
   32  git clone git@github.com:weable-kosa/kosa-msa-2024-1st.git
   33  ls
   34  cd kosa-msa-2024-1st/
   35  ls
   36  docker run -d --name wordpress_db -e MYSQL_ROOT_PASSWORD=1234 -e MYSQL_DATABASE=wordpress mysql:5.7
   37  docekr run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress --link wordpressdb:mysql -p 80:80 wordpress
   38  docke run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress --link wordpressdb:mysql -p 80:80 wordpress
   39  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress --link wordpressdb:mysql -p 80:80 wordpress
   40  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress --link wordpress_db:mysql -p 80:80 wordpress
   41  docker prot wordpress
   42  docker port wordpress
   43  docker port wordpress_db
   44  docker run -d --name worpress_db_host_volumn -e MYSQL_ROOT_PASSWORD=1234 -e MYSQL_DATA
   45  docker run -d --name worpress_db_host_volumn -e MYSQL_ROOT_PASSWORD=1234 -e MYSQL_DATABASE=wordpress -v /home/wordpress_db:/var/lib/mysql mysql:5.7
   46  docker logs wordpress_db_host_volumn
   47  docker ps
   48  docker run -d --name wordpress_db_host_volumn -e MYSQL_ROOT_PASSWORD=1234 -e MYSQL_DATABASE=wordpress -v /home/wordpress_db:/var/lib/mysql mysql:5.7
   49  docker logs wordpress_db_host_volumn
   50  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_Db_host_volumn:mysql -p 80:80 wordpress
   51  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_db_host_volumn:mysql -p 80:80 wordpress
   52  docekr ps
   53  docker ps
   54  docker stop wordpress
   55  docker ps
   56  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_db_host_volumn:mysql -p 80:80 wordpress
   57  docker ps
   58  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_db_host_volumn:mysql -p 80:80 wordpress
   59  docker rm wordpress_host_volumn
   60  docekr 
   61  docker rm wordpress_host_volumn
   62  docker rm wordpress_Db
   63  docker rm wordpress_db
   64  docekr stop wordpress_db
   65  docker stop wordpress_db
   66  docker rm wordpress_db
   67  docker ps
   68  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_db_host_volumn:mysql -p 80:80 wordpress
   69  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_db_host_volumn:mysql:. -p 80:80 wordpress
   70  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=1234 --name wordpress_host_volumn --link wordpress_db_host_volumn:mysql:5.7 -p 80:80 wordpress
   71  docker ps
   72  docker stop word_db_host_volumn
   73  docker stop wordpress_db_host_volumn
   74  docker rm wordpress_db_host_volumn
   75  docker run -d --name wordpressdb_hostvolume -e MYSQL_ROOT_PASSWORD=password -e MYSQL_DATABASE=wordpress -v /home/wordpress_db:/var/lib/mysql mysql:5.7~
   76  docker run -d --name wordpressdb_hostvolume -e MYSQL_ROOT_PASSWORD=password -e MYSQL_DATABASE=wordpress -v /home/wordpress_db:/var/lib/mysql mysql:5.7
   77  docker run -d -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=password --name wordpress_hostvolume --link wordpressdb_hostvolume:mysql -p 80:80 wordpress:5.6
   78  docker ps
   79  cd /var
   80  ls
   81  cd lib
   82  cd mysql
   83  ls
   84  cd mysql
   85  ls
   86  cd /home
   87  ls
   88  cd /var/lib
   89  ls
   90  cd docker
   91  ls
   92  volumes
   93  cd volumes
   94  ls
   95  docekr logs wordpressdb_hostvolumn
   96  docker logs wordpressdb_hostvolumn
   97  docekr ps
   98  docker ps
   99  docker stop wordpress_db_host_volumn
  100  docker ps
  101  docker stop wordpress_db_host_volumn
  102  docker rm -f wordpress_db_host_volumn
  103  docker ps
  104  docker rm -f worpress_db_host_volumn
  105  docker ps
  106  docker rm -f wordpress_hostvolumn
  107  docker rm -f wordpress_hostvolume
  108  clear
  109  cd /
  110  cd ~/work
  111  ls
  112  touch stack.yaml
  113  ls
  114  vi stack.yaml
  115  docker-compose -f stack.yml up
  116  apt install docker-compose
  117  docker-compose -f stack.yml up
  118  docker-compose -f stack.yaml up
  119  clear
  120  docker ps
  121  docker-compose -f stack.yaml up
  122  cd work
  123  ls
  124  docker-compose -f stack.yaml up
  125  docker-compose -f -d stack.yaml up
  126  docker-compose -f -d stack.yaml create
  127  docker-compose stack.yaml create
  128  docker-compose creaet
  129  docker-compose create
  130  docker-compose create stack.yaml
  131  rm stack.yaml
  132  clear
  133  touch
  134  touch docker-compose.yaml
  135  vi docker-compose.yaml
  136  docker-compose create
  137  docker ps
  138  docker-compose up
  139  docker-compose down
  140  docker-compose up
  141  docker-compose up -d
  142  docker ps
  143  vi docker-compose.yaml 
  144  cat docker-compose.yaml 
  145  docker compose down
  146  docker-compose up -d
  147  history
  148  cat docker-compose.yaml 
  149  docker compose stop
  150  docker-compose start
  151  cat docker-compose.yaml 
  152  docker-compose down
  153  docker-compose up -d
  154  cd /var/lib/mysql
  155  cd /var/lib
  156  mkdir mysql
  157  cd /var/www/html
  158  cd /var/www
  159  cd /var
  160  mkdir www
  161  cd www
  162  mkir html
  163  mkdit html
  164  mkdir html
  165  cd ~/work
  166  ls
  167  docker-compose down
  168  docekr-compose up
  169  docker-compose up
  170  docker-compose down
  171  docker-compose up
  172  docker-compose down
  173  docker-compose up
  174  docker-compose down
  175  docker-compose up
  176  ls
  177  cd ~/work
  178  vi docker-compose.yaml 
  179  cd ~/work
  180  ls
  181  vi docker-compose.yaml 
  182  cat docker-compose.yaml 
  183  docker-compose up
  184  docker-compose dwon
  185  docker-compose down
  186  docker-compose up
  187  docker-compose down
  188  vi docker-compose.yaml 
  189  cat docker-compose.yaml 
  190  docker-compose down
  191  docker-compose up
  192  docker-compose down
  193  docker-compose up
  194  docker-compose down
  195  vi docker-compose.yaml 
  196  docker-compose down
  197  docker-compose up
  198  docker-compose down
  199  vi docker-compose.yaml 
  200  docker-compose up
  201  docker-compose down
  202  vi docker-compose.yaml 
  203  docker-compose up
  204  docker-compose down
  205  vi docker-compose.yaml 
  206  docker-compose up
  207  vi docker-compose.yaml 
  208  docker-compose up
  209  docker-compose down
  210  vi docker-compose.yaml 
  211  docker-compose down
  212  vi docker-compose.yaml 
  213  docker-compose up
  214  docker-compose down
  215  vi docker-compose.yaml 
  216  docker-compose up
  217  vi docker-compose.yaml 
  218  docker-compose down
  219  docker run -d --name joomla_db -e MYSQL_ROOT_PASSWORD=password -e MYSQL_DATABASE=joomla_db -v /home/joomla_db:/var/lib/mysql mysql:5.7
  220  docker run -d --name joomla -p 80:80 --link joomla_db:mysql -e JOOMLA_DB_HOST=joomla_db -e JOOMLA_DB_USER=root -e JOOMLA_DB_PASSWORD=password -e JOOMLA_DB_NAME=joomla_db -v /home/joomla_web:/var/www/html joomla:4.4
  221  vi docker-compose.yaml 
  222  docker-compose up
  223  docker-compose down
  224  docker-compose up
  225  docekr ps
  226  docker ps
  227  docekr rm -f joomla
  228  docker rm -f joomla
  229  docker rm -f joomla_db
  230  docker-compose up
  231  docker ps
  232  docker rm joomla
  233  docker rm -f joomla
  234  docker rm -f joomla_db
  235  docker run -it --name commit_test ubuntu:14.4
  236  docker run -it --name commit_test ubuntu:14.04
  237  clear
  238  docker commit -a "aj" -m "init" commit_test commit_test:init
  239  docekr images
  240  docker images
  241  docekr tun -it --name commit_test2 commit_test
  242  docker run -it --name commit_test2 commit_test:init
  243  docker ps
  244  exit
  245  docker inspect ubuntu:14.04
  246  docker inspect commit_test:init
  247  docker inspect wordpress
  248  docker rm -f ${docker ps -a -q}
  249  docker rm -f $(docker ps -a -q)
  250  docker ps -a -q
  251  docker ps -a
  252  clear
  253  docker run -it --name commit_container1 ubuntu:14.04
  254  docker commit commit_container1 frozengrape:0.0
  255  docker ps
  256  docker images
  257  docker tag frozengrape:0.0 frozengrape/frozengrape:0.0
  258  docker images
  259  docker login
  260  docker push frozengrape/frozengrape:0.0
  261  docker images
  262  docekr image rm -f frozengrape
  263  docker image rm -f frozengrape
  264  docker image rm -f frozengrape:0.0
  265  docker image rm -f frozengrape/frozengrape:0.0
  266  docker images
  267  docekr run -it frozengrape/frozengrape:0.0
  268  docker run -it frozengrape/frozengrape:0.0
  269  docker image rm -f frozengrape/frozengrape:0.0
  270  docker ps
  271  docker
  272  docker ps
  273  docker run -d --name myregistry -p 5000:5000 --restart=always registry:2.6
  274  clear
  275  docker ps
  276  docker logs myregistry
  277  docker image
  278  docker images
  279  docker pull frozengrape:0.0
  280  docker pull frozengrape/frozengrape:0.0
  281  ifconfig
  282  ipconifg
  283  ipconfig
  284  ifconfig
  285  apt install net-tools
  286  ifconfig
  287  cd /usr/lib
  288  cd systemd
  289  cd system
  290  vi docker.service
  291  vi /etc/default/docker
  292  systemctl daemon-reload
  293  systemctl restart docker
  294  docekr push 172.17.0.2:5000/frozengrape/frozengrape:0.0
  295  docker push 172.17.0.2:5000/frozengrape/frozengrape:0.0
  296  clear
  297  cd 
  298  docker rm -f $(docker ps -a -q)
  299  mkdir ~/dockerfile
  300  cd dockerfile/
  301  touch test.html
  302  ls
  303  vi Dockerfile
  304  ls
  305  docker build -t mybuild:0.0 ./
  306  docker images
  307  docker run -d -p 80:80 --name myserver mybuild:0.0
  308  history
```