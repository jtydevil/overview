# 环境初始化

## Composer 安装
#### 全局安装
````
curl -sS https://getcomposer.org/installer | php
mv composer.phar /usr/local/bin/composer

# 设置全局path
# 打印路径：composer global config bin-dir --absolute
vim ~/.bash_profile
export PATH=${PATH}:~/.composer/vendor/bin/

# 设置国内镜像
composer config -g repo.packagist composer https://packagist.phpcomposer.com
````

## IDE - PHPStorm
- [下载安装](https://www.jetbrains.com/phpstorm/)
- [破解](http://idea.lanyus.com/)
- 安装插件：PhpStorm -> Preferences -> Plugins -> Browse repositories...

### 必装插件
- [PHP_CS](../dev/rule/phpcs.md)
- [PHP_MD](../dev/rule/phpmd.md)
- Laravel 智能提示
    - 安装插件Laravel Plugin
    - composer require --dev barryvdh/laravel-ide-helper
    - bootstrap/app.php 中注册provider
        ````
        $app->register(\Barryvdh\LaravelIdeHelper\IdeHelperServiceProvider::class);
        ````
    - 生成提示文件
        ````
        php artisan ide-helper:generate
        php artisan ide-helper:meta
        ````
    - 重启phpstorm，启动插件
        ````
        PhpStorm -> Preferences -> Languages & Frameworks -> PHP -> Laravel（勾选两个选项）
        ````
- [xdebug](init/xdebug.md)：断点调试
- Swagger Plugin：智能提示swagger yaml文档编写
