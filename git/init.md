#### 1. cd到要绑定的文件目录



#### 2. 生成本地git管理

```js
git init
```



#### 3.  添加需要提交的文件

```
git add .
```



#### 4. 输入github邮箱

```js
git config --global user.email "yanyong995821@gmail.com"
```



#### 5.  提交文件到本地库

```js
git commit -m "first commit"
```



#### 6. 本地仓库关联github仓库

```js
git remote add origin https://github.com/yanyong995821/accumulate.git
```



#### 7. 推送到远端代码库

```js
git push -u origin main
```
