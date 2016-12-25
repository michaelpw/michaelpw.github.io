<?php

require_once('lib/paymentwall.php');
$params = array(
    'key'=>'d3b6fef35b283a32c5b92bc6d2a37dc3',
    'uid'=>'57ccc60dc9b8841c3aee8dda',
    'widget'=>'p1_1',
    'email' => 'test@paymentwall.com',
    'history[registration_date]' => '1477267200',
    'sign_version'=>3
);

$paramsoffer = array(
    'key'=>'d3b6fef35b283a32c5b92bc6d2a37dc3',
    'uid'=>'57ccc60dc9b8841c3aee8dda',
    'widget'=>'w6_1',
    'email' => 'test@paymentwall.com',
    'history[registration_date]' => '1477267200',
    'sign_version'=>3
);

Paymentwall_Config::getInstance()->set(array('private_key' => 'dce5da7c341aef630abe808f5dc60cae'));
$params['sign'] = (new Paymentwall_Signature_Widget())->calculate(
    $params,
    $params['sign_version']
);

$widget = 'https://api.paymentwall.com/api/ps?'.http_build_query($params);

Paymentwall_Config::getInstance()->set(array('private_key' => 'dce5da7c341aef630abe808f5dc60cae'));
$paramsoffer['sign'] = (new Paymentwall_Signature_Widget())->calculate(
    $paramsoffer,
    $paramsoffer['sign_version']
);

$widgetoffer = 'https://api.paymentwall.com/api/?'.http_build_query($paramsoffer);

?>

<html>
    <body>
        <h1>Paymentwall Virtual Currency API Iframe Widget Call Example</h1>
        <h2>BUY/DONATE Virtual Currency with Paymentwall</h2>
        <iframe src="<?php echo $widget; ?>" width="750" height="500" frameborder="0"></iframe>
        <h2>EARN Virtual Currency with Paymentwall</h2>
        <iframe src="<?php echo $widgetoffer; ?>" width="750" height="800" frameborder="0"></iframe>
    </body>
</html>