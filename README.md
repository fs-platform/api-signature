## signature

- 对接口请求进行签名验证
- 本拓展满足psr2,psr4 规范
- 已通过单元测试

## 基本使用
1. 安装
```bash
$ composer require aron/signagture-verification
```

2. 发布config 文件
```bash
$ php artisan vendor:publish
```

4. 开始使用
```php
\Signature::verifySignature('时间戳',
'随机字符串','requestBody', '签名认证key','客户端签名');

app('Signature')->verifySignature('时间戳',
'随机字符串','requestBody', '签名认证key','客户端签名');
```
