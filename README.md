# drf-auth-stryds
Backend Server providing REST API for authentication

# API List
| Method      	| URL 				| Params     				| Description 			|
| :---        	| :---   			| :--- 						| :--- 					|
| GET      		| accounts/data/    |  Authorization Token  	| Currently Logged in User's Info|
| GET      		| accounts/users/   |    						| List of All Users registered |
| POST     		| accounts/users/   |   first_name, last_name, email, password, gender, birth_date | Create a new user |
| PATCH/PUT     | accounts/users/<pk>|    						| Update user details |
| POST   		| token/login       | email, password      		| Login |
| POST   		| token/logout      | auth_token      			| Logout |

# Technical Stacks
- Python/Django
- DRF(Django-Rest-Framework)
- django-cors-header
- heroku