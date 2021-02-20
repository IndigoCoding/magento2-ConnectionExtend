# Magento 2 [Indigo Connection Extend](http://indigocoding.work) Extension

---

This extension helps with using multiple user-defined connections/resources for declarative schema instead of only the 
3 default resources (default, checkout, sales).

This extension is to be used by developers for easier development. Work with both Magento 2 Open Source and 
Commerce.

---

## Requirements
Magento 2.3+ (Tested with Magento 2.3.0 EE, 2.3.4 CE and 2.4.0 CE)

## ✓ Install via [composer](https://getcomposer.org/download/) (recommended)
Run the following command under your Magento 2 root dir:

```
composer require indigo/module-connection-extend
php bin/magento maintenance:enable
php bin/magento setup:upgrade
php bin/magento setup:di:compile
php bin/magento setup:static-content:deploy
php bin/magento maintenance:disable
php bin/magento cache:flush
```

## Install manually under app/code
1. Download & place the contents of this repository under {YOUR-MAGENTO2-ROOT-DIR}/app/code/Indigo/ConnectionExtend  
2. Run the following commands under your Magento 2 root dir:
```
php bin/magento maintenance:enable
php bin/magento setup:upgrade
php bin/magento setup:di:compile
php bin/magento setup:static-content:deploy
php bin/magento maintenance:disable
php bin/magento cache:flush
```

## Usage

After the installation, Go to The Magento 2 admin panel

Go to Stores -> Settings -> Configuration, under tab Advanced -> System -> Connection Extend Configuration. In
Connection Extend List setting, enter the list of resource name as string, separated by a comma.

Setup new connection and resource by modifying app/etc/env.php file (new resource key must be the same as configured 
above)

Put the new resource name in db_schema.xml file whenever needed and enjoy!

---

http://indigocoding.work/

Copyright © 2021 IndigoCoding. All rights reserved.  