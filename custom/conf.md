# 配置二次开发目录

将**config/compatible.php**复制到**config/production/compatible.php**并且修改配置
```php
 <?php
 //二次开发目录设置,`custom`可以替换为自己的二次开发目录
 //如果该配置已开启，并且有对应的目录，则表示已经开启二次开发目录
 define('CUSTOM_CORE_DIR', ROOT_DIR.'/custom');
```
新建目录custom，需要和app目录同级
```shell
drwxr-xr-x  38 www  www   1292  8  5 22:21 app
drwxr-xr-x   7 www  www    238  8 24 19:38 bootstrap
drwxrwxrwx  33 www  www   1122  8 24 12:00 config
drwxr-xr-x   3 www  www    102  8 25 13:57 custom //和app目录同级
```