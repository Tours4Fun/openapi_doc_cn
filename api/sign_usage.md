	<?php
	
	$app_key = 'your_app_key';
	
	$app_secret = 'your_app_secret';
	
	$t = time();
	
	$http_body = array(
		'product_id' => 1234
	);
	
	$sign = md5( $app_key . $t . $app_secret . json_encode($http_body) );
	
	// Do http request ...
	
	
	?>