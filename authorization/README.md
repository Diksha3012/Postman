// authorization--------------------------------------------------------------------------------------------------------------




Applyting few authorization tools in APIs------------------
------------------------------------------------------------------------------------------------------------------------------------------------------------------------
(1)Basic authorizaion:
--------------------------------------------
Basic authorizaion means we just have to pass username and password.

              1.create a get request under this API name authorization and pass the url https://postman-echo.com/basic-auth and send 
     
               you may see response as unauthorized" and status is 401 unauthorized.

		2. create anotherget request or edit previously get request> the go to authorization tab>select basic auth>pass uername  "postman" and password  		                   "password"

		now send the request and see the response.

			the output will be and status will be 200k
                 
                                   {
                                        "authenticated": true
                                     }
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
(2) API key
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
                      1.go create an get request>pass url this api.openweathermap.org/data/2.5/forecast/daily?q=Delhi&cnt=1 and send empty in authorization you must                                     see response



  					{
   					 "cod": 401,
    						"message": "Invalid API key. Please see http://openweathermap.org/faq#error401 for more info."

                                for:// api key authentication failure
														}
                        
                      2. (1). go to openweather.com>API>current weather data>api doc>by city name>copy first address>api.openweathermap.org/data/2.5/weather?q={city                                name}&appid={API key}
                                           
                                         on this address click on api key>generate.( in my case i generated f33c9764eee78c9eea28f24144224c98)



                           (2) now go back to authrorization colletion>create get request> at url write this >api.openweathermap.org/data/2.5/weather?q=london


                                 then go to authorization>select type>api key>

                                           key::id
                                           value::f33c9764eee78c9eea28f24144224c98
                                           add to: query params

                                  and then send the request and response will come 200 K

                                 for://api key succession
