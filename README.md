# VisaAPICalls
First of visa developer obtain a user
https://developer.visa.com
# Install
```sh
include './vendor/autoload.php';

$apiKey = '*******';
$secret = '*******';
$body = json_encode([
    'amount' => '10',
    'currency' => 'USD',
    'payment' => [
        'cardNumber' => '378282246310005',
        'cardExpirationMonth' => '10',
        'cardExpirationYear' => '2016',
    ]
        ]);
$CyberSourcePayments = new \VisaCyberSourcePayments\CyberSourcePayments($apiKey, $secret, $body);
$json = $CyberSourcePayments->payments();
```



