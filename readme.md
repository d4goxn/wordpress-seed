# WordPress Seed

A WordPress install with example config files: Apache virtual host config and a hosts file.

* URL: wordpress-seed.local
* Web root, hardcoded: /home/dan/Projects/wordpress-seed/www

## After Cloning

* Give web root to Apache: `sudo chown www-data:www-data www -R`.
* Give yourself write group write permission in the web root: `sudo chmod g+w www -R`.
* Update paths and urls in the config templates to match your desired project struture.
* Insert the hosts file contents into your `/etc/hosts`.
* Copy the virtualhost config file to `/etc/apache2/sites-available`.

## Requirements

* You must be in the same group as apache: `usermod -aG www-data [you]`. After adding yourself, you must reboot in order for the chanes to take effect.

## TODO:

Installer using Grunt and wp-cli. [wp-cli](http://wp-cli.org/) is pretty cool on its own, but I would like to be able to set up a WP site with a single command + config file + prompts.
