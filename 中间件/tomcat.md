# Tomcat

## Tomcat基础

### Web概念

- 软件架构：

  - C/S：客户端/服务器端
  
  - B/S：浏览器/服务器端

- 静态资源：
  - 静态资源：所有用户访问后，得到的结果都是一样的，称为静态资源，静态资源可以直接被浏览器解析。如果：html、css、JavaScript、jpg……
  - 动态资源：每个用户访问相同资源后，得到的结果可能不一样，称为动态资源。动态资源转换为静态资源，再返回给浏览器，通过浏览器进行解析。如：Serverlet/jsp、php、asp……

- 网络通信三要素：
  - IP：电子设备（计算机）在网络中的唯一标识。
  - 端口：应用程序在计算机中的唯一标识。
  - 传输协议：规定了数据传输的规则
  
---

### 常见的Web服务器

- 概念：

  - 服务器：安装了服务器软件的计算机
  - 服务器软件：接受用户的请求，处理请求，做出响应
  - Web服务器软件：接受用户请求，处理请求，做出响应【在Web服务器软件中，可以部署Web项目，让用户通过浏览器来访问这些项目】
  
| Web服务器 | 特点 |
| --- | --- |
| Apache HTTP Server | 开源，支持多种协议，高性能，可扩展性，易用性 |
| Nginx | 轻量级，高性能，高并发性，稳定性 |
| Microsoft Internet Information Services (IIS) | 易用性，安全性，适用于Windows平台 |
| Lighttpd | 轻量级，高性能，高并发性，稳定性 |
| Node.js | 高性能，高并发性，易用性，适用于各种场景 |
| Apache Tomcat | 开源，主要用于开发和部署Java Web应用程序，支持Servlet、JSP、EL和JavaBean等技术 |
| Jetty | 主要用于开发和部署Java Web应用程序，支持Servlet、JSP、EL和JavaBean等技术，高性能，可扩展性，易用性 |
| GlassFish | 主要用于开发和部署Java EE应用程序，支持Java EE规范，高性能，可扩展性，易用性 |
| WildFly | 主要用于开发和部署Java EE应用程序，支持Java EE规范，高性能，可扩展性，易用性 |

- Tomcat安装
下载链接：[Tomcat下载链接](https://tomcat.apache.org/download-80.cgi)

- Tomcat目录结构

| 目录 | 说明 |
| --- | --- |
| bin | 存放Tomcat的启动、停止等批处理脚本文件 |
| conf | 用于存放Tomcat的相关配置文件 |
| lib | Tomcat服务器的依赖包 |
| logs | Tomcat默认的日志存放目录 |
| webapps | Tomcat默认的Web应用部署目录 |
| work | Web应用JSP代码生成和编译的临时文件 |

- Tomcat启动停止

| 操作 | 说明 |
| --- | --- |
| 启动 | 双击 bin/startup.bat 文件 |
| 停止 | 双击 bin/shutdown.bat文件 |
| 访问 | 直接浏览器输入 <http://localhost:8080> |
