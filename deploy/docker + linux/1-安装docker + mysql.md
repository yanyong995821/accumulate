##### 安装Docker

```js
 curl -fsSL https://test.docker.com -o test-docker.sh
 
 sudo sh test-docker.sh

 // 查看镜像
 docker images 
```



##### 安装mysql

```js
 // 安装
 docker pull mysql:latest 
 
 // 将mysql运行到docker容器中
 docker run -itd --name yy-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=yq245304 mysql
 
 // 进入mysql容器中
 docker exec -it yy-mysql bash
```



##### 配置mysql

```mysql
# 登入
mysql -u root -p
ALTER USER 'root'@'localhost' IDENTIFIED BY 'yq245304';

# 添加远程可访问用户
CREATE USER 'yy'@'%' IDENTIFIED WITH mysql_native_password BY 'yy123';
GRANT ALL PRIVILEGES ON *.* TO 'yy'@'%';
```



运行jar包
docker run -d -p 8080:8080 -v /yy/yy.jar:/yy/yy.jar --name apringboot java:8u111 java -jar /yy/yy.jar