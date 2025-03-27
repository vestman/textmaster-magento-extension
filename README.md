# Textmaster module for Magento 2

Also available on the Magento marketplace: https://marketplace.magento.com/

## Summary
Get your product, category, page and block attributes translated by professionals directly through Magento.

## Description
TextMaster makes it easy to translate your entire product, category, page and block attrinutes by professionals in over 15 languages. Open your doors to new markets in just a few clicks by using our intuitive extension to make your store multilingual.

## Requirements
This module supports Magento 2 version
* 2.3.x 
* 2.4.x
* 2.5.x

### How to use

1. Install the module via Composer :

``` composer require textmaster/module-textmaster ```

2. Enable it

``` bin/magento module:enable TextMaster_TextMaster ```

3. Install the module and rebuild the DI cache

``` bin/magento setup:upgrade ```

### MySQL 5.7 and MariaDB ROW_NUMBER() compatibility

If you're running MySQL 5.7 or a MariaDB version that doesn't support the ROW_NUMBER() window function, you'll need to apply a compatibility patch:

1. Locate the patch file in the module: `/etc/patches/textmaster-mariadb-rownumber-retro-compatibility-fix.patch`
2. Copy it to your Magento installation's patches directory:
```sh
cp textmaster-mariadb-rownumber-retro-compatibility-fix.patch [patches-directory-path]
```
3. Run Magento's setup upgrade:
```
bin/magento setup:upgrade
```

### How to configure

> TEXTMASTER > Configuration > Authentication

> TEXTMASTER > Configuration > Language Mapping

> TEXTMASTER > Configuration > Translatable Content Selection
