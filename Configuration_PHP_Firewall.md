PHP Firewall configuration


You can active or deactive most protections in PHP Firewall.


Open the php-firewall/firewall.php


All the parameters are between the lines 27 and 53

  * true = active
  * false = deactive


```
  define('PHP_FIREWALL_ADMIN_MAIL', '' );  // write your email, php firewall mail you  each attack detected
  define('PHP_FIREWALL_PUSH_MAIL', false ); // active email rapport true or false deactive
  define('PHP_FIREWALL_LOG_FILE', 'logs' );  // filename logs for php firewall
  define('PHP_FIREWALL_PROTECTION_RANGE_IP_DENY', true ); // IPs reserved blocker
  define('PHP_FIREWALL_PROTECTION_RANGE_IP_SPAM', true );  // IPs spam blocker
  define('PHP_FIREWALL_PROTECTION_URL', true );  // URL protection
  define('PHP_FIREWALL_PROTECTION_REQUEST_SERVER', true ); // Request protection
  define('PHP_FIREWALL_PROTECTION_SANTY', true ); // Santy worm protection
  define('PHP_FIREWALL_PROTECTION_BOTS', true ); // Bad bots protection
  define('PHP_FIREWALL_PROTECTION_REQUEST_METHOD', true ); // Bad method protection
  define('PHP_FIREWALL_PROTECTION_DOS', true ); // Mini dos protection
  define('PHP_FIREWALL_PROTECTION_UNION_SQL', true ); // Union sql protection
  define('PHP_FIREWALL_PROTECTION_CLICK_ATTACK', true ); // Include files protection
  define('PHP_FIREWALL_PROTECTION_XSS_ATTACK', true ); // XSS protection
  define('PHP_FIREWALL_PROTECTION_COOKIES', true ); // sanitize cookies
  define('PHP_FIREWALL_PROTECTION_POST', true ); // Sanitize POST vars
  define('PHP_FIREWALL_PROTECTION_GET', true );  // sanitize GET vars
```