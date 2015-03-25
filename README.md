# Magento Facebook Remarketing and Conversion Tracking
Facebook Remarketing and Conversion Tracking Extension for Magento.

## Installation ##

Magento Facebook Remarketing and Conversion Tracking uses [Composer](http://getcomposer.org) and [Magento Composer Installer](https://github.com/magento-hackathon/magento-composer-installer) to handle installation of the module and its dependencies. To install Magento Facebook Remarketing and Conversion Tracking you will need a copy of _composer.phar_ in your path. If you do not have it availble, run the following commands from your terminal.

    $ curl -sS https://getcomposer.org/installer | php
    $ chmod a+x composer.phar

If you are already using Magento Composer Installer and have an existing _composer.json_, add _https://github.com/deved-it/magento-keen-io_ to the repositories list and _deved-it/magento-keen-io_ as a required dependency for your project. That's it!

If you do not have an existing Magento Composer Installer _composer.json_ file defined, you can use the following template.

    {
      "repositories": [
          {
            "type":"composer",
            "url":"http://packages.firegento.com"
          },
          {
            "type": "vcs",
            "url": "https://github.com/deved-it/FacebookRemarketingJs"
          }
      ],
      "require": {
          "magento-hackathon/magento-composer-installer": "*",
          "deved-it/facebookremarketingjs": "*"
      },
      "extra":{
          "magento-root-dir":"./",
          "magento-force":"true"
      }
    }


To install Magento Facebook Remarketing and Conversion Tracking and its dependencies just run composer.phar.

    $ ./composer.phar install

#After Installing

- Clear Cache
- Log out and log back in
- Goto System -> Config -> MagePal -> Facebook Remarketing API
