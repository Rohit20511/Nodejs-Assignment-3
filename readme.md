#Assignment #3 Pizza-delivery

API for a pizza-delivery company that accepts orders.

Requirements are :-
create a web app that allows customers to:

1. Signup on the site

2. View all the items available to order

3. Fill up a shopping cart

4. Place an order (with fake credit card credentials), and receive an email receipt

The all methods are :- 

1. Get Account Details(GET Method)

http://localhost:3000/users/?email=rjboy@gmail.com

HEADERS
Content-Type      application/json
token             to0y4g8b5xcvcdja89gs

PARAMS           
email			  rjboy@gmail.com

BODY
{
	"email": "rjboy@gmail.com"
}

2. Login to Account(POST Method)

http://localhost:3000/tokens/

HEADERS
Content-Type		application/json
BODY
{
	"email": "rjboy@gmail.com",
	"password": "123456"
}

3. Get token details(GET Method)

http://localhost:3000/tokens/?id=fy97a7m5upt63ibrsk5i

HEADERS

Content-Type		application/json
token			to0y4g8b5xcvcdja89gs

PARAMS
id			uiqljzfpufpis6q8l7sr

BODY
{
	"email": "rjboy@gmail.com",
	"password": "123456"
}

4. Extend Token Expiry (PUT Method)
 
HEADERS
Content-Type		application/json
token               to0y4g8b5xcvcdja89gs
PARAMS
id	                uiqljzfpufpis6q8l7sr
BODY
{
	"id": "uiqljzfpufpis6q8l7sr",
	"extend": true
}

5. Delete Token (DEL Method)

http://localhost:3000/tokens/?id=cv97d7m5uyj63ibjik5i

HEADERS
Content-Type		application/json
token				to0y4g8b5xcvcdja89gs
PARAMS
id                   uiqljzfpufpis6q8l7sr
BODY
{
	"id": "uiqljzfpufpis6q8l7sr"
}


6. Get Food Items (GET Method)

http://localhost:3000/foods?email=rjboy@gmail.com
Get all the food items and pizza on the system.

HEADERS

Content-Type		application/json
token			    to0y4g8b5xcvcdja89gs
PARAMS
email               	rjboy@gmail.com
BODY
{
	"id": "uiqljzfpufpis6q8l7sr"
}

7. Add food item to cart (POST Method)

http://localhost:3000/cart

HEADERS
Content-Type		application/json
token			to0y4g8b5xcvcdja89gs

BODY
{
	"item": 1,
	"quantity":3
}

8. Get all items in cart(GET Method)

http://localhost:3000/cart

HEADERS
Content-Type		application/json
token			to0y4g8b5xcvcdja89gs
BODY
{
	"item": 1,
	"quantity":3
}

9. Update Cart Item(PUT Method)
http://localhost:3000/cart

HEADERS
Content-Type			application/json
token				to0y4g8b5xcvcdja89gs
BODY
{
	"id": "uiqljzfpufpis6q8l7sr",
	"quantity":2
}

10. Delete Cart Item (PUT Method)

http://localhost:3000/cart
Delete cart item

HEADERS
Content-Type			application/json
token				to0y4g8b5xcvcdja89gs
BODY
{
	"id": "uiqljzfpufpis6q8l7sr"
}

11. Make Final Orders(POST Method)

http://localhost:3000/orders

HEADERS
Content-Type		application/json
token			    to0y4g8b5xcvcdja89gs
BODY
{
	"email": "rjboy@gmail.com"
}

12. Register Account(POST Method)

http://localhost:3000/users/

HEADERS
Content-Type            application/json
BODY
	{
	"email": "rjboy@gmail.com",
	"name": "Rohit Jaiswal",
	"address": "indore ,india",
	"password": "123456"
	}



