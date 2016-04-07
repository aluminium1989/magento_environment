# magento_environment
magento testing environment
pre-installed app: composer

0. composer update.
1. copy build.properties.dist to build.properties
2. leave the version which you are working on: instances.versions = magento112
3. modify instance configuration:
instances.magento112.version = magecorelab-magento-ee-1.12
instances.magento112.folder = /cymbio112 # relative the current dir.
4. run phing n98_install (setup magerun)
5. phing setup_project (install selected in p3 magento versions)
6. phing deploy_module (deploy module through magento instances)
