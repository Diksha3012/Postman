- go to https://reqres.in/   """use this dummy api for testing"""'
     1. create a collection (API chaining) and use get request tp get all users data.((https://reqres.in/api/users?page=2)) and 
     then click on send. as a reponse we will get all the  users data.
     2.Now create Put request under API chaining collection .put this address on address (https://reqres.in/api/users/2) ..
      this is put  so we must pass request payload and copy the payload from (https://reqres.in/api/users/2) 
       and send. i have send this payload {    "name": "morpheus",    "job": "zion resident"}        

     3. go to API chaining collecion>three dots>variable>username 

     4. Copy all the response of get request of API chaining into json path finder extension and find the path of Machael
     5. go to get request of API chaining  and than write test code there like this


                        jsonData=JSON.parse(responseBody);
			value==jsonData.data[0].first_name;
			pm.globals.set("username","value");

     6. now go to put request of API chaining in the body part of put request we can refer that value like this
       
                  	      {
    				"name": "{{username}}",
<<<<<<< HEAD
   			        "job": "zion resident"
				}
=======
   					 "job": "zion resident"
				}
>>>>>>> 5a92fcb30fe2b94b1ef71dcf809e70bbb9ab22fe
