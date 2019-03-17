# cocos2d-x v3.15中的js例子tests

## 一、项目测试运行
因为cocos2d-x中的js-tests中的路径有问题，所以js项目没有办法跑起来，这里单独把修改好的例出来了

打开运行web项目有三种方式：

#### 1.使用cocos run命令

``` bash
#cd到项目目录下，使用下边令命就可以打开web项目的服务器
cocos run -p web
```

在浏览器里输入
```
http://127.0.0.1:8000
```
即可打开js-test项目

#### 2.使用nodejs的http服务器模块

可以参考下边说明为项目建一个https服务器，前提是你的系统中已经安装了nodejs：

https://www.jianshu.com/p/800e1e423df6

#### 3.使用其他的web服务器

可以使用其他的各种web服务器，像python的SimpleHTTPServer建一个https服务器

## 二、项目发布到网站服务器

对于最终发布，使用cocos compile这个命令

```bash
#同样是项目目录下运行下边命令
cocos compile -p web -m release
```

这时会在项目目录下生成一个publish目录，把里边的内容复制到你的网站服务器就可以了