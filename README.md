### Aop插件使用教程

> 同时支持直接new和从容器获取需要被切入的对象，也支持三方库的切入vendor目录下的类方法， 在不改变现有代码的情况下切入需要切入的前置后置方法，用在统计http请求，Rpc，组件链路追踪，日志记录，统计函数耗时 修改函数返回结果的应用场景

#### 安装

```
composer require xiaoyangguang/aop
```

1. 配置config\plugin\xiaoyangguang\aop\aop.php文件  
2. 自定义切入类需要实现Xiaoyangguang\Aop\AspectInterface接口并配置到以上aop配置文件中
3. 最后启动服务，并测试。


```shell
php start.php start
curl  http://127.0.0.1:8787
此时控制台打印前置和后置切面函数打印值
```


