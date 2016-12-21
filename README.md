<a href="https://www.captchasolutions.com/"><img src="https://www.captchasolutions.com/img/captchasolutions.png"></a>

# Bypass Captcha / Captcha Solver / Decaptcha
A RESTful Captcha Solver or Bypass Captcha Service

Solving at a rate of $0.99 per 1000 captchas solved.

Check out http://www.captchasolutions.com

----
Usage

```php
<?php
	include ('lib/CaptchaSolutions.php');
	
	$image = 'http://www.captchacreator.com/files/captchac_code.php';
	
	$key = "[<YOUR API KEY]"; // Get your own key at https://www.captchasolutions.com/register/
	$secret = "[<YOUR SECRET KEY]"; // Get your own key at https://www.captchasolutions.com/register/	

	$api = new CaptchaSolutions($key, $secret);
	
	// Get available balance
	print $api->balance('sptest');
	
	// Simple captcha image decode via URL
	print $api->decode($image);	
	
	// Google's NoCaptcha
	print $api->nocaptcha('6LcT6wATAAAAAMBYUbtdHChwcLt3kaoBpvICxdDj', 'https://www.isnare.com/login.php');	
	
	//Text Captcha Decoding
	print $api->text('What color is the sky?');		
```

----
Sponsors:

- https://www.captchasolutions.com/
- https://www.isnare.com/
- https://articlefr.cf/
- http://allwomencentral.com/
- http://submito.us/
