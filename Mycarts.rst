
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
*{"user_id": "25"},{"products":[{"product_id":"397","amount":"1"},{"product_id":"398","amount":"1"}]*

Note: if user_id is empty, the API will create an anonymous cart and will return the token to refer to that cart.

===
PUT
===
Update existing cart: 

*PUT api.php?_d=mycarts&ajax_custom=1*
*{"user_id": "25"},{"products":{"1867885166":{"product_id":"397","amount":"2"}}*

Note: user_id is a reference to an existing user, or a token referring to an anonymous cart.

======
DELETE
======
Remove certain product from cart

*DELETE api.php?_d=mycarts/4293572607&ajax_custom=1*

Clear cart

*DELETE api.php?_d=mycarts&ajax_custom=1*
