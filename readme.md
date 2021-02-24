# Arrow Magento Module

Help shoppers checkout in one click with Arrow.
This is a standard Magento module and can be installed under `app/code/arrow`

## Merchant Account

To use Arrow you need a merchant account with a Payment Service Provider and sign for Arrow at projectarrow.co

## Installation

Pull this repo into your Magento directory under `app/code/arrow`.

1. Enable the Arrow module:
```
bin/magento module:enable Arrow
```

2. After enabling the module upgrade your database:
```
bin/magento setup:upgrade
```

3. And deploy:
```
bin/magento setup:static-content:deploy
```

4. After deploying the cache make sure to compile again:
```
bin/magento setup:di:compile
```

## Debug

Include this at the top of your index.php in `pub/index.php` to see all errors in Magento:
```
ini_set('display_errors', 1);
error_reporting(E_ALL);
```