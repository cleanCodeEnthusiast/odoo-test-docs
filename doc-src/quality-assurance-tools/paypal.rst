Paypal testing
==============

To test paypal payments you need to:

* Create developer account
* Add seller and buyer in developer sandbox
* Configure odoo
* Directly testing

Create developer account
^^^^^^^^^^^^^^^^^^^^^^^^

Go to https://developer.paypal.com/ and create new account.

Add seller and buyer
^^^^^^^^^^^^^^^^^^^^

* Go to **Dashboard->Sand box->Accounts**. Create business (seller) and personal (buyer) accounts. It's recommended to don't use non-ascii symbols in account information (address, name etc.)
* Add some money to buyer (type amount in according field).
* Go to http://sandbox.paypal.com and login as seller. May be you will be forced to apply unconfirmed ssl certificate.
* Follow odoo docs: https://www.odoo.com/documentation/user/14.0/general/payment_acquirers/paypal.html


Configure odoo
^^^^^^^^^^^^^^

* Install **payment_paypal** module
* Go to **Settings->Payments->Payments->Paypal**.
* Pres **Edit**.
* Enter here **Paypal Email ID** - it is *seller* account.
* Follow odoo docs: https://www.odoo.com/documentation/user/14.0/general/payment_acquirers/paypal.html

Directly testing
^^^^^^^^^^^^^^^^

Open web shop. Buy some goods and pay with paypal. When you will be redirected on paypal page use *buyer* login and password.
