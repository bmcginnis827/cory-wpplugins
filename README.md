SSH in and switch to root: `sudo su`

Navigate into wordpress directory: `/var/www/html/wordpress`

Edit wp-config.php: `nano wp-config.php`

Change this line `define('WP_HTTP_BLOCK_EXTERNAL', true);` to `define('WP_HTTP_BLOCK_EXTERNAL', false);` 

Exit and save: `Ctrl + X` then press `Y`

Navigate into htdocs: `cd /var/www/html/wordpress/htdocs`

Run this command to install your plugin: `wp plugin install https://downloads.wordpress.org/plugin/advanced-ads.1.34.0.zip --activate --allow-root --url=darknetdaily.com` (**Note:** you can get the downloads URL from the download button on the WordPress downloads site)

Edit wp-config.php again: `cd .. && nano wp-config.php`

Change this line `define('WP_HTTP_BLOCK_EXTERNAL', false);` back to to `define('WP_HTTP_BLOCK_EXTERNAL', true);` 

Exit and save: `Ctrl + X` then press `Y`
