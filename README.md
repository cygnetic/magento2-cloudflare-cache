# Turiknox Cloudflare Cache

## Overview

A Magento 2 module that purges Cloudflare cache when flushing the cache storage in the Magento admin.

## Requirements

Magento 2.1.x, 2.2.x

## Installation

Copy the contents of the module into your Magento root directory.

Enable the module via the command line:

/path/to/php bin/magento module:enable Turiknox_CloudflareCache

Run the database upgrade via the command line:

/path/to/php bin/magento setup:upgrade

Run the compile command and refresh the Magento cache:

/path/to/php bin/magento setup:di:compile
/path/to/php bin/magento cache:clean

## Usage

Head to Stores -> Configuration -> Advanced -> Developer -> Purge Cloudflare Cache to enable the module and add your Cloudflare credentials.

System -> Cache Management, and click on the 'Flush Cache Storage' button.
