# sms_integration_package-sms_integration
sms integrations
#installation

` composer require sms_integration_package/sms_integration:dev-master `

after complete installation open `config/app.php`

put in  this provider array 

```php

Sms\Integration\Package\SmsProvider::class
```
and in aliase add this

```php
"SendSmsIntegration"=>Sms\Integration\Package\SendSms::class

```

now run this command in command
`php artisan vendor:publish `

to usage this message

`SendSmsIntegration::SendSms(mobile_number,message,0); `
