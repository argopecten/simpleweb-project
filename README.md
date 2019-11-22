# Composer template for Drupal projects

Simpleweb platform with Drupal 8 on Aegir 3, with composer
This project template provides the Simpleweb platform with [Drupal 8](https://www.drupal.org/) on [Aegir 3](https://www.aegirproject.org), using [Composer](https://getcomposer.org/).

## Usage

First you need to [install Aegir](https://www.aegirproject.org).

Then, with this composer template, you can create a Simpleweb platform in your Aegir at https://example.com/node/add/platform:

* name the platform as you wish, i.e.: `1.0.1+8.7.9`
* select `Deploy a Composer project from a Git repository`
* Docroot: `web`
* Git URL: `https://github.com/argopecten/simpleweb-project`
* Branch/tag: `1.0.1` or [any other tags from the repository](https://github.com/argopecten/simpleweb-project/releases)

## What does the template do?

When installing the given `composer.json` of this template, some tasks are taken care of:

* [Drupal 8](https://drupal.org) will be installed in the `web`-directory.
* The Simpleweb profile will be installed in the `web/profiles`-directory and all the built-in drupal profiles will be removed.
* Modules (packages of type `drupal-module`) will be placed in `web/sites/all/modules/contrib/`
* Theme (packages of type `drupal-module`) will be placed in `web/sites/all/themes/contrib/`
* Latest version of drush is installed locally for use at `vendor/bin/drush`.
