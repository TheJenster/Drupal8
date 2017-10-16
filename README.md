# govCMS 8 project template for Platform.sh

This project provides a starter kit for govCMS 8 projects hosted on [Platform.sh](http://platform.sh). 

## Starting a new project

To start a new govCMS 8 project on Platform.sh:

1) Clone or download this project.

2) Create a new project on Platform.sh (you may like to use the Australian region). When given the option to add your own code, upload your project code via git.

## Managing a Drupal site built with Composer

Once the site is installed, there is no difference between a site hosted on Platform.sh
and a site hosted anywhere else.  It's just Composer.  See the [Drupal documentation](https://www.drupal.org/node/2404989) for tips on how best to leverage Composer with Drupal 8.

## How does this starter kit differ from vanilla Drupal from Drupal.org?

1. The `vendor` directory (where non-Drupal code lives) and the `config` directory
   (used for syncing configuration from development to production) are outside
   the web root. This is a bit more secure as those files are now not web-accessible.

2. The `settings.php` and `settings.platformsh.php` files are provided by
   default. The `settings.platformsh.php` file automatically sets up the database connection on Platform.sh, and allows controlling Drupal configuration from environment variables.

3. We include recommended `.platform.app.yaml` and `.platform` files that should suffice
   for most use cases. You are free to tweak them as needed for your particular site.
