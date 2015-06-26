# yii2-authclient-instagram
Instagram client for yii2-authclient

## Installation
Through Composer
From console:
```
composer require brainsrage/yii2-authclient-instagram
```
or add to "require" section to composer.json
```
"brainsrage/yii2-authclient-instagram": "dev-master"
```
##Usage
Register your application [in Instagram](http://instagram.com/developer/clients/register)

and add the Instagram client to your auth clients.

```
php
'components' => [
    'authClientCollection' => [
        'class' => 'yii\authclient\Collection',
        'clients' => [
            'instagram' => [
                'class' => 'app\common\auth\Instagram',
                'clientId' => 'Instagram client id',
                'clientSecret' => 'Instagram client secret',
            ],
            // other clients
        ],
    ],
    // ...
 ]
```
