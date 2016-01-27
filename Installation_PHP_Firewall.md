PHP Firewall install in your website ( or CMS, Blog, Forum, Galery ... )

  * Upload the folder php-firewall/
  * put the php-firewall/logs.txt in writable chmod
  * Open the main file ( index.php for example ) and add these lines juste after the < ?php


```
define('PHP_FIREWALL_REQUEST_URI', strip_tags( $_SERVER['REQUEST_URI'] ) );
define('PHP_FIREWALL_ACTIVATION', true );
if ( is_file( @dirname(__FILE__).'/php-firewall/firewall.php' ) )
	include_once( @dirname(__FILE__).'/php-firewall/firewall.php' );
```



if you want deactive PHP Firewall, edit this line:
```
define('PHP_FIREWALL_ACTIVATION', false );
```