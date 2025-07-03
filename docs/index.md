# Welcome to filamentWallet documentation

The first step in the installation process is to make sure that your server has all the prerequisites necessary to host filamentWallet. Most server with Cpanel already have all the prerequisites included.

##**Server requirements**

- PHP >= 8.3.\*
- PDO PHP Extension
- Tokenizer PHP Extension
- PHP Fileinfo extension
- OpenSSL PHP Extension
- XML PHP Extension
- Mbstring PHP Extension
- GD Library
- CURL Library
- PHP mod_rewrite enabled
- A server that supports Symlinks

## **Upload files, create a database and an email with cpanel**

- Upload The filamentWallet zip file to your server's `public_html/` folder.
- Create a database and write-down the database name, user , and password for [step 2](#step-2)
- Import the .sql to your recently created databse. Use your cpanel phpMyadmin
- Create an email account and write-down the email's `smtp` info for [step 2](#step-2)

## **Setting enviroment variables**

- In your server go to `.. /public_html/application/.env` and edit the .env file

[![image00](img/dotenv.png)](img/dotenv.png)
