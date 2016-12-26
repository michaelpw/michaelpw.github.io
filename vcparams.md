## Virtual Currency API

Virtual Currency API is the best choice for you when your business allows your customers to be able to **[BUY](https://api.paymentwall.com/api/ps?key=d3b6fef35b283a32c5b92bc6d2a37dc3&uid=user1102&widget=p1_1&sign_version=3&email=example%40paymentwall.com&history%5Bregistration_date%5D=1477267200&sign=fad77829aff32f623fbb37a727a1f854e809efa7d5725a593af03fd4a60b49b6) and [EARN](https://api.paymentwall.com/api/?key=d3b6fef35b283a32c5b92bc6d2a37dc3&uid=user1102&widget=w6_1&sign_version=3&email=example%40paymentwall.com&history%5Bregistration_date%5D=1477267200&sign=1c0784ed6afdb90318c1c7dcc0b765b81413edc8f407b3034754d3d16c9dd810)** coins, points, credits and any other kinds of virtual currency.

---

### Widget call

Paymentwall widget can be displayed as an __*[iframe](https://paymentwall-php-jeokim.c9users.io/iframe.php)*__ on your website / application or opened up as a __*[new page](https://paymentwall-php-jeokim.c9users.io/vc.html)*__.

>**Parameters**

<p>* Required Parameters</p>

| Name   | Type |Description |
| :------| :---- |:-----------|
|<i>*key</i> |string|eg: d3b6fef35b283a32c5b92bc6d2a37dc3 <br> Log in to your Merchant Account to get the Project Key in General Settings of the project.|
|<i>*uid</i> |string|eg: user1102 <br> Assigned ID of the end-user in your system who is viewing the widget. The ID must be unique per user. <br>The maximum length is 64 characters.|
|<i>*widget</i> |string|eg: p1_1, p10_1, m2_1 <br> Can be created and obtained in the Widgets section of your project.|
|<i>*email</i> |string|eg: test@paymentwall.com <br>Email of end-user.<br>Paymentwall will automatically send a receipt to the user once the payment / offer is completed.|
|<i>*timestamp</i> |string(10)|eg: 1477267200 <br> Unix Timestamp of the current date.<br>Maximum length is 10.|
|<i>*sign_version</i> |int|eg: 2, 3 <br> Signature version.<br>Version 2 employs MD5 and version 3 utilizes SHA256.|
|<i>*sign</i> |string|The signature of the widget.<br>Refer to [Signature Calculation](1) for more details.|
|<i>evaluation</i> |string|The value could be either 0 or 1.<br>If 1, the widget can be loaded without having to log into the Merchant Account. Applied on test environment only.|
|<i>country_code</i> |string(2)|The length must be 2-character according to ISO 3166-1 alpha-2 code of the country.<br>Overrides the default geological location of user. Requires widget signature.|
|<i>vcr</i> |int|eg: 10, 100 etc <br>The amount of virtual currency is exchanged for one unit of real currency.<br>Overrides the setting for currency exchange rate in your project. Can be activated per request.|
|<i>vcc</i> |string|eg: USD, EUR <br>The code of the real currency.<br>Overrides the setting in your project. For example, if vcc=EUR, vcr=100 then 1 EUR can buy 100 virtual currency for your project. Can be activated per request.|
|<i>vc</i> |string|eg: Coins, Points, Credits <br>Name of the virtual currency<br>Overrides the setting in your project. Can be activated per request.|
|<i>pingback_url</i> |string|eg: http://yourdomain.com/pingback <br>URL of pingback listener script where pingback requests are sent to<br>Overrides the Pingback URL setting in your project. Can be activated per request.|
|<i>success_url</i> |string|eg: http://yourdomain.com/paymentsuccess <br>URL of the page where users should be redirected to after the payment is completed.|
|<i>promo</i> |string|eg: promo[0]=[type]=percent_bonus, promo[0][discount]=50,promo[0][minimum_amount]=2.95,promo[0][minimum_amount_currency]=EUR will add 50% of the amount of virtual currency for all prices that are greater than or equal to 2.95 EUR<br>Requires signed widget call with sign_version=3|
