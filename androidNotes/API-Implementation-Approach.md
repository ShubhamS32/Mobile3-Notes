# API Implementation Approach 

This doc is prepared to guide you while working with Web APIs
An API can have XML or JSON as a response type.
Below structure will guide you how a standard JSON API response will look like.

================================================================

* Development Server Url : http://10.0.0.100/apis
* Testing Server Url : https://fanrag-test.weboapps.com/apis
* Production Server Url : https://fanrag.com/apis
* Request Type : GET/POST (POST is ideal)
* Response Type : JSON

You can have a following error codes to identify the status of your request you made to the server.
200 - OK
400 - Error
500 - Internal server error
404 - Action not found

# 1) API Name : User registration
## URL : /signup
### Request Parameters (Mentioning data type is not mandatory)
* firstName         (String)     First Name of User
* lastName          (String)     Last Name of User
* emailAddress      (String)     A valid email id
* password          (String)     Password
* gender            (String)     Gender of user (m/f)
 

### Expected Responses
### 1) Success : 
	{
    		"status": 200,
	   	"message": "Registration successful,please check your email for verification code."
	}
### 2 ) Failure :
	{
		"status": 400,
		"message": "No data to process.”
	}


# 2) API Name : Get All Leagues
## URL : /getAllLeagues
### Request Parameters : Do not specify anything if API doesn't require request parameters
### Expected Responses
### 1) Success : 
	{
    	  "status": 200,
    	  "message": "Success",
    	  "data": [
        		{
			   "leagueId": 1,
			   "leagueName": "NFL"
        		},
        		{
           		   "leagueId": 2,
            		   "leagueName": "NHL"
			},
			{
            		   "leagueId": 3,
            		   "leagueName": "NASCAR"
			}
    		]
	 }
### 2) If no user exists : 
       {
    	"status": 200,
    	"message": "No records exists",
    	"data": [ ]
       }
### 3 ) Failure :
       {
	"status": 400,
	"message": "No data to process.”
       }
