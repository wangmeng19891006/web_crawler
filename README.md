# web_crawler

# 基于node的爬虫

# 功能

### 1 可以将指定的页面，指定的相同结构的数据爬取下来，成为接口在线使用
### 2 可以使用get请求，通过传入不同的id来获取相同结构页面的数据
### 3 已做跨域设置，端口号默认3003，服务器已测试可用

# 使用方法：

### 1 安装依赖
`npm i`

### 2 使用pm2/node 挂载index.js

`node index.js`


# 注意：

#### 如果想要存到文件,把注释的代码打开。

#### 如果要爬需要cookie验证的网站
写法：

```
//可以用set设置cookie
//网页的cookie可以通过控制台 document.cookie获取
 let cookie = "这里是cookie"
 superagent.get(url).set("Cookie",cookie).end()
```

#### 如果需要爬带有header
写法：
```
//可以用set设置头部信息
request.get('/search').set('API-Key', 'foobar').set('Accept', 'application/json');
```