Welcome to phpWallet documentation
=================

The first step in the installation process is to make sure that your server has all the prerequisites necessary to host phpWallet. Most server with Cpanel already have all the prerequisites included.

##__Server requirements__
* PHP >= 7.1.*
* PDO PHP Extension
* Tokenizer PHP Extension
* PHP Fileinfo extension
* OpenSSL PHP Extension
* XML PHP Extension
* Mbstring PHP Extension
* GD Library
* CURL Library
* PHP mod_rewrite enabled
* A server that supports Symlinks

## __Upload files, create a database and an email with cpanel__

* Upload The phpWallet zip file to your server's ` public_html/ ` folder.
* Create a database and write-down the database name, user , and password for [step 2](#step-2)
* Import the .sql to your recently created databse. Use your cpanel  phpMyadmin
* Create an email account and write-down the email's ` smtp ` info for [step 2](#step-2)

## __Setting enviroment variables__

* In your server go to ` .. /public_html/application/.env ` and edit the .env file

[![image00](img/dotenv.png)](img/dotenv.png)

## __The file storage__

* Copy the symbolic link folder ` storage ` from ` .. /public_html/application/public/ `  to ` .. /public_html/ `

[![image01](img/storage_link.png)](img/storage_link.png)

## __Configuring PayPal__
### Add PayPal API keys

* go to ` .. /public_html/application/config/paypal.php ` and edit the paypal.php file

[![image02](img/paypal_config.png)](img/paypal_config.png)
### Activate PayPal Gateway

* go to ` www.yourwebsite.com/admin ` and login with an admin account, then activate the PayPal gateway in settings menu

[![image03](img/paypal_gateway_setting.png)](img/paypal_gateway_setting.png)

## __Configuring Paystack__
### Add Paystack API keys

* go to ` .. /public_html/application/http/controllers/PaystackController.php ` and edit the PaystackController.php file

[![image04](img/paystack_config.png)](img/paystack_config.png)

### Activate Paystack Gateway 
* Activate the Paystack gateway in settings menu. ( process described [here](#step-2_1)  )

## __Configuring Stripe__
### Add Stripe API keys

* Set ` STRIPE_PUBLISHABLE_KEY ` and ` STRIPE_SECRET_KEY `  ( line 26 and 27 ) in the .env file described in [step 2](#step-2) 

### Activate Stripe Gateway 
* Activate the Stripe gateway in settings menu. ( process described [here](#step-2_1)  )