# Lumen ApiHander
Lumen Api 异常处理类

### 安装
```shell
composer require "hongjh/lumen-ucenter"
```
### 配置
在 <app-path>/bootstrap/app.php 40-45行左右，替换
```
$app->singleton(
    Illuminate\Contracts\Debug\ExceptionHandler::class,
    Hongjh\Exceptions\ApiHandler::class
);
```
