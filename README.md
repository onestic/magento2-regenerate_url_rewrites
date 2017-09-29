Regenerate a Url rewrites of products/categories
=====================

Magento 2 "Regenerate Url rewrites" extension add a CLI feature which allow to regenerate a Url rewrites of products/categories in all stores or specific store.

## INSTALLATION

### MANUAL INSTALLATION
* extract files from an archive

* deploy files into Magento2 folder `app/code/OlegKoval/RegenerateUrlRewrites`

### ENABLE EXTENSION
* enable extension (in command line, see manual: `http://devdocs.magento.com/guides/v2.0/config-guide/cli/config-cli-subcommands.html`):
>`$> bin/magento module:enable OlegKoval_RegenerateUrlRewrites`

* to make sure that the enabled module is properly registered, run 'setup:upgrade':
>`$> bin/magento setup:upgrade`

* [if needed] re-deploy static view files:
>`$> bin/magento setup:static-content:deploy`


## HOW TO USE IT:
* to re-generate all Url rewrites of the categories/products in all stores (it support a multistores) run:
>`$> bin/magento ok:urlrewrites:regenerate`

* to regenerate all Url rewrites of the categories/products in the specific store view (e.g.: store view id is "2"):
>`$> bin/magento ok:urlrewrites:regenerate 2`

Enjoy!

Best regards,
Oleg Koval