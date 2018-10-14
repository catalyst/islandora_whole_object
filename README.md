# Islandora Whole Object

## Introduction

An first attempt at addressing https://github.com/Islandora-CLAW/CLAW/issues/886. Mainly me learning how to to understand Islandora's data structures and render them in a Drupal 8 module.

## Requirements

* [Islandora](https://github.com/Islandora-CLAW/islandora) aka CLAW
* [Devel](https://www.drupal.org/project/devel)

## Installation

1. Clone this repo into your CLAW's `drupal/web/modules/contrib` directory.
1. Enable the module either under the "Admin > Extend" menu or by running `drush en -y islandora_whole_object`.

## Usage

After you enable this module, a new tab will appear (for users with 'administer site configuration' permission) on objects:

![Whole object menu tab](docs/menu.png)

Clicking the link will show you the JSON-LD of the current object:

![JSON-LD](docs/jsonld.png)

You will then see the JSON-LD for the specified object.

## To do

* Make the tab appear only on nodes with the 'islandora_object' content type; make the content type configurable
* Format the content so it's more useful, andby remove our dependency on Devel
* Add more than just the JSON-LD (e.g., thumnails of media, etc.)
* Add the option of showing the content in a block instead of as a tab

## Maintainers

Current maintainers:

* [Mark Jordan](https://github.com/mjordan)

## License

[GPLv2](http://www.gnu.org/licenses/gpl-2.0.txt)
