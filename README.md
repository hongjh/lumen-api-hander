# Lumen ApiHander
Lumen Api 异常处理类

### 安装
```shell
composer require "hongjh/lumen-api-hander"
```
### 配置
在 <app-path>/bootstrap/app.php 40-45行左右，替换
```
$app->singleton(
    Illuminate\Contracts\Debug\ExceptionHandler::class,
    Hongjh\Exceptions\ApiHandler::class
);
```

### 开启调试模式
``` 
设置 .env APP_DEBUG=true, 并在
在 HTTP 报头加上 Accept = text/html，会显示错误栈
```