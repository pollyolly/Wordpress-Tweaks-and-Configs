Reset admin password 

1. Access phpmyadmin
2. In wp_users update username and passwords. 
```
UPDATE `wp_users` SET `user_pass` = MD5( 'new_password' ) WHERE `wp_users`.`user_login` = "admin_username";
```
3. Now, access the wp-login.php in the url.

Reset Woocommerce / Remove all data, products, orders 
```
define( 'WC_REMOVE_ALL_DATA', true ); //wpconfig
```
Fix Slow Elementor Page Editor
```
define( 'WP_MEMORY_LIMIT', '256M' );//Add memory limit
```
