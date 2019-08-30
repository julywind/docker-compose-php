
# 1、保证你的 83 是没被占用的

# 2、拷贝
  cp .env.example .env 并设置你自己的

# 设置建议如下：

# mac 下，以下的 linfeng 你需要换成你自己的名字。
DIR_WWW=/Users/linfeng/data/www/

# centOS 下
DIR_WWW=/data/www/

# 3、运行
docker-compose up -d

# 4、其他常用命令
  docker-compose ps
  docker-compose down
  docker-compose restart -d
  docker exec -it ct-phpfpm bash


# 目录解释
1. .env.example - *Env variable file template.*
2. ./Dockerfile - *Phpfpm docker mirror build file.*
3. ./docker-compose.yml - *Docker marshals file.*
4. ./docker-compose.build.yml - *Docker marshals file.(Local building)*
5. ./conf/mysql/mysql.cnf - *MySQL configuration.*
6. ./conf/nginx/nginx.conf - *Nginx configuration.*
7. ./conf/nginx/conf.d - *Nginx site configuration directory.*
8. ./conf/php/php.ini - *PHP configuration.*
10. ./log/nginx - *Nginx log file.*
11. ./log/supervisor - *Supervisor log file.*
12. ./files - *163 Mirrors URL.*

