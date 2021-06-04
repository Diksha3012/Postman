(3)Bearer Token authorization
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
                     1.) go to authorization collection>get request>enter url http://httpbin.org/bearer and then go to authorizaion tab>bearer token> enter token                          santosh and send.

                                for///:bearer token with false token


                     2.)  (a) go to github.com account>settting>developer setting>personal access token>generate new token> generated>ok


                              Note:copy the generated token
 

                           (b) go to github Docs>references>Respositories
 					  From here:list repositories for authenticated user and you may see the path in curl shell or with http get/post method below                                                
                              

                           (c) go to postman>collection>Github collection>get method>enter url "https://api.github.com/user/repos"
                                   
                                select authorizarion>select bearer token>In token paste the generated token values and send.
                      
----------------------------------------------------------------------------------------------------------------------------------------------------------------------- 




   

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

(4)OAuth2.0
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------				1.)As we have generated our token from github.com by generate new token.We can use the same token for Oauth2.0 authorization as well.

			2.)go to github Docs>references>Respositories:
		         
			From here:list repositories for authenticated user and you may see the path in curl shell or with http get/post method below                                                
			go to postman>collection>Github collection>get method>enter url "https://api.github.com/user/repos"

       			select authorizarion>oauth2.0>select available token>then paste in access token and send.