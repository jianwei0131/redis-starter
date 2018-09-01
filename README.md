# redis-starter

## 介绍
该项目的主要目的是为了快速配置redis工具类,并且基于springboot的自动配置,来快速引入到需要的项目中.

## 内容

项目的中主要是将以前自己写的redis工具类(https://github.com/cdy1996/common-util),通过快速的配置引入到项目中,主要是通过spring的自动配置来实现.

当然目前只将单redis的工具类引入,主从和集群的redis工具类并未加入(其实也差不多),留待之后再添加.

## 使用

在springbootApplication 的main类上,加上@EnableRedisUtil注解,然后在配置文件中配置redis的地址

## 设计

主要时通过@configuration进行bean的配置,然后通过@import导入到容器中.