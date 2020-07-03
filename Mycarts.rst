
Mycarts
=======
*Mycarts* is a custom API method to handle customer carts.

URL
===
https://hetvoedselcollectief.nl/api.php?_d=mycarts&ajax_custom=1 


Supported operations
====================
===
GET
===
Get cart contents

*GET api.php?_d=mycarts&ajax_custom=1*

====
POST
====
Create cart and add products

*POST api.php?_d=mycarts&ajax_custom=1*
*{"products":[{"product_id":"397","amount":"1"},{"product_id":"398","amount":"1"}]*

===
PUT
===
Update existing cart: 

*PUT api.php?_d=mycarts&ajax_custom=1*
*{"products":{"1867885166":{"product_id":"397","amount":"2"}}*

======
DELETE
======
Remove certain product from cart

*DELETE api.php?_d=mycarts/4293572607&ajax_custom=1*

Clear cart

*DELETE api.php?_d=mycarts&ajax_custom=1*
