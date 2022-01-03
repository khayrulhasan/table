## Ans One
# Create a file named “ main.php" in your directory.
### Run this command in your root directory terminal CMD: composer require khayrulhasan/table
``` php

<?php 
# file name : main.php
use Khayrulhasan\Table\User;
use Khayrulhasan\Table\UserCollection;

require_once "vendor/autoload.php";

/*
 *  data(s)
 */

$user1 = new User(1, 'Selim Reza', 'me@selimreza.com');
$user2 = new User(2, 'Half Way', 'selimppc@gmail.com');
$data = new UserCollection([$user1, $user2]);


/*
 * final output
 */
$data->displayAsTable();

