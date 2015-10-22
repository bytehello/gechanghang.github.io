#HTTP协议简要
HTTP是开发中经常用到的从网路获取数据的一种通信协议。

##HTTP简单介绍
在移动开发中，client（手机端）是发送消息给server（服务器），而且永远是手机端发送给服务器端。手机端不向服务器发送数据，服务器也就不会返回数据

跟SOCKET最主要的区别就是：socket是一种手机端和服务器端的连接不断开的协议，打个比方，QQ的服务器会与手机建立socket通信，确保一有消息，就会发送给客户端。

##HTTP请求

HTTP主要常用分为两种
- GET : 就是从服务器索取数据
- POST : 提交数据给服务器，让服务器返回数据

**HTTP的请求格式如下**
```
<request-line>
<request-header>
<blank-line>
<request-body>
```
说明:第一行必须是一个请求行(request-line),用来说明请求类型,要访问的资源以及所使用的HTTP版本.
 紧接着是一个首部(header)小节,用来说明服务器要使用的附加信息.
  之后是一个空行.
再后面可以添加任意的其他数据**称之为主体(body)**.



HTTP请求包含了**请求头(header)** 和 **请求体(body)**
body只有对POST才有效。
请求头里面包括了一些请求的参数，是以**key:value**的形式
形如
```
Accept: text/html
Accept-Charset: GBK,utf-8
Accept-Encoding: gzip.deflate
Accept-Language:zh-CN,zh;
```
而请求体包含了要提交给服务器的数据，形如
```
username=gch&pwd=gechanghang
```
##HTTP响应

与请求相对应的就是响应，同样的，也包括了响应头和响应体。

**HTTP响应格式如下**
```
<status-line>
<header>
<blank-line>
<body>
```
HTTP状态码如果为200，则表示为一切正常。



