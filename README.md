# Magento 2 GeoIP Database Extension by Magefan

[![Total Downloads](https://poser.pugx.org/magefan/module-geoip/downloads)](https://packagist.org/packages/magefan/module-geoip)
[![Latest Stable Version](https://poser.pugx.org/magefan/module-geoip/v/stable)](https://packagist.org/packages/magefan/module-geoip)

<a href="https://savelife.in.ua/en/donate-en/#donate-army-card-monthly"><img width="830" height="208" src="https://cm.magefan.com/blog/support-ukraine.png"></a>

<img width="150" height="100" src="https://magefan.com/media/wysiwyg/made_in_ukraine.jpg">


This Magento 2 GeoIP module provides you PHP methods for getting customer country by IP, without any additional plugin for PHP.

It is used for [Magento 2 Currency Auto Switcher](https://magefan.com/magento-2-currency-switcher-auto-currency-by-country) and [Magento 2 Auto Language Switcher](https://magefan.com/magento-2-auto-language-switcher) by Magefan


## Requirements
  * Magento Community Edition 2.0.x-2.4.x or Magento Enterprise Edition 2.0.x-2.4.x

## Installation Method 1 - Installing via composer
  * Open command line
  * Using command "cd" navigate to your magento2 root directory
  * Run command: composer require magefan/module-geoip
```
composer require magefan/module-geoip
php bin/magento setup:upgrade
php bin/magento setup:di:compile
php bin/magento setup:static-content:deploy
```


## Installation Method 2 - Installing using archive
  * Install GeoIP2 PHP API (https://github.com/maxmind/GeoIP2-php).
  * Download [ZIP Archive](https://github.com/magefan/module-geoip/archive/master.zip)
  * Extract files
  * In your Magento 2 root directory create folder app/code/Magefan/GeoIp
  * Copy files and folders from archive to that folder
  * In command line, using "cd", navigate to your Magento 2 root directory
  * Run commands:
```
php bin/magento setup:upgrade
php bin/magento setup:di:compile
php bin/magento setup:static-content:deploy
```

## How To Use
```
protected $ipToCountryRepository;

public function __construct(
    \Magefan\GeoIp\Model\IpToCountryRepository $ipToCountryRepository,
    ....//other code
) {
    $this->ipToCountryRepository = $ipToCountryRepository;
    ...//other code
}

public function example() {
    $visitorCountyCode = $this->ipToCountryRepository->getVisitorCountryCode();
    $someCountryCodeByIp = $this->ipToCountryRepository->getCountryCode('104.27.164.57');
    ...//other code
}
```

## Support
If you have any issues, please [contact us](mailto:support@magefan.com)
then if you still need help, open a bug report in GitHub's
[issue tracker](https://github.com/magefan/module-geoip/issues).

## Need More Features?
Please contact us to get a quote
https://magefan.com/contact

## License
The code is licensed under [Open Software License ("OSL") v. 3.0](http://opensource.org/licenses/osl-3.0.php).

This product includes GeoLite2 data created by MaxMind, available from
<a href="https://www.maxmind.com">https://www.maxmind.com</a>.

## Originaly use this databases:
https://www.maxmind.com

http://software77.net/geo-ip/


## [Magento 2 Extensions](https://magefan.com/magento-2-extensions) by Magefan

### [Magento 2 Admin Panel Extensions](https://magefan.com/magento-2-extensions/admin-extensions)

  * [Magento 2 Edit Order Extension](https://magefan.com/magento-2-edit-order-extension)
  * [Magento 2 Better Order Grid Extension](https://magefan.com/magento-2-better-order-grid-extension)
  * [Magento 2 Extended Product Grid](https://magefan.com/magento-2-product-grid-inline-editor)
  * [Magento 2 Product Tabs Extension](https://magefan.com/magento-2/extensions/product-tabs)
  * [Magento 2 Facebook Pixel Extension](https://magefan.com/magento-2-facebook-pixel-extension)
  * [Magento 2 Email Attachments](https://magefan.com/magento-2-email-attachments)
  * [Magento 2 Admin View Extension](https://magefan.com/magento-2-admin-view-extension)
  * [Magento 2 Admin Email Notifications](https://magefan.com/magento-2-admin-email-notifications)
  * [Magento 2 Login As Customer Extension](https://magefan.com/login-as-customer-magento-2-extension)

### [Magento 2 Google Extensions](https://magefan.com/magento-2-extensions/google-extensions)

  * [Magento 2 Google Indexing API](https://magefan.com/magento-2-google-indexing-api)
  * [Magento 2 Google Analytics 4 Extension](https://magefan.com/magento-2-google-analytics-4)
  * [Magento 2 Google Tag Manager](https://magefan.com/magento-2-google-tag-manager)
  * [Magento 2 Google Shopping Feed](https://magefan.com/magento-2-google-shopping-feed-extension)
  * [Magento 2 Google Customer Reviews](https://magefan.com/magento-2-google-customer-reviews)

### [Magento 2 SEO Extensions](https://magefan.com/magento-2-extensions/magento-2-seo-extensions)

  * [Magento 2 SEO Extension](https://magefan.com/magento-2-seo-extension)
  * [Magento 2 Rich Snippets Extension](https://magefan.com/magento-2-rich-snippets)
  * [Magento 2 HTML Sitemap Extension](https://magefan.com/magento-2-html-sitemap-extension)
  * [Magento 2 XML Sitemap Extension](https://magefan.com/magento-2-xml-sitemap-extension)
  * [Magento 2 Twitter Cards Extension](https://magefan.com/magento-2-twitter-cards-extension)
  * [Magento 2 Facebook Open Graph Extension](https://magefan.com/magento-2-open-graph-extension-og-tags)

### [Magento 2 Blog Extensions](https://magefan.com/magento-2-extensions/blog-extensions)

  * [Magento 2 Blog Extension](https://magefan.com/magento2-blog-extension)
  * [Magento 2 Blog Plus Extension](https://magefan.com/magento2-blog-extension/pricing)
  * [Magento 2 Blog Extra Extension](https://magefan.com/magento2-blog-extension/pricing)
  * [Magento 2 Multi Blog Extension](https://magefan.com/magento-2-multi-blog-extension)
  * [Magento 2 Product Widget Advanced Extension](https://magefan.com/magento-2-product-widget)

### [Magento 2 Marketing Automation Extensions](https://magefan.com/magento-2-extensions/magento-marketing-automation)

* [Magento 2 Dynamic Categories](https://magefan.com/magento-2-dynamic-categories)
* [Magento 2 CMS Display Rules Extension](https://magefan.com/magento-2-cms-display-rules-extension)
* [Magento 2 Automatic Related Products](https://magefan.com/magento-2-automatic-related-products)
* [Magento 2 Price History](https://magefan.com/magento-2-price-history)
* [Magento 2 Mautic Integration Extension](https://magefan.com/magento-2-mautic-extension)
* [Magento 2 YouTube Widget Extension](https://magefan.com/magento2-youtube-extension)
    
 
### [Magento 2 Cart Extensions](https://magefan.com/magento-2-extensions/cart-extensions)

  * [Better Magento 2 Checkout Extension](https://magefan.com/better-magento-2-checkout-extension)
  * [Magento 2 Coupon Code Link](https://magefan.com/magento-2-coupon-code-link)
  * [Magento 2 Convert Guest to Customer Extension](https://magefan.com/magento2-convert-guest-to-customer)

### [Magento 2 Speed Optimization Extensions](https://magefan.com/magento-2-extensions/speed-optimization-extensions)

  * [Magento 2 Lazy Load Extension](https://magefan.com/magento-2-image-lazy-load-extension)
  * [Magento 2 WebP Optimized Images Extension](https://magefan.com/magento-2-webp-optimized-images)
  * [Magento 2 Rocket JavaScript Extension](https://magefan.com/rocket-javascript-deferred-javascript)

### [Magento 2 Multi-Language Extensions](https://magefan.com/magento-2-extensions/multi-language-extensions)

  * [Magento 2 Hreflang Tags Extension](https://magefan.com/magento2-alternate-hreflang-extension)
  * [Magento 2 Auto Currency Switcher Extension](https://magefan.com/magento-2-currency-switcher-auto-currency-by-country)
  * [Magento 2 Auto Language Switcher Extension](https://magefan.com/magento-2-auto-language-switcher)
  * [Magento 2 GeoIP Switcher Extension](https://magefan.com/magento-2-geoip-switcher-extension)
  * [Magento 2 Translation Extension](https://magefan.com/magento-2-translation-extension)

### Developers Tools

  * [Magento 2 Zero Downtime Deployment](https://magefan.com/blog/magento-2-zero-downtime-deployment)
  * [Magento 2 Cron Schedule](https://magefan.com/magento-2-cron-schedule)
  * [Magento 2 CLI Extension](https://magefan.com/magento2-cli-extension)
  * [Magento 2 Conflict Detector Extension](https://magefan.com/magento2-conflict-detector)

  ### Magento 2 Point of Sale

  * [Magento 2 POS System](https://magefan.com/magento-pos-system)

  ### Magento 2 Theme

  * [Optimized Magento 2 Theme](https://magefan.com/optimized-magento-2-theme)
   
  ### Shopify Apps

  * [Shopify Login As Customer](https://apps.shopify.com/login-as-customer)
  * [Shopify Blog](https://apps.shopify.com/magefan-blog)
  
  ### Shopware Extensions
  
  * [Shopware WebP Extension](https://magefan.com/shopware/extensions/webp)
  * [Shopware Blog Extension](https://magefan.com/shopware/extensions/blog)
