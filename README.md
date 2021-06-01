 # Postman....................
 - Fake Api creation(own api)

1.Install nodejs("in my case already installed)(node --version)

2.npm comes by default with nodejs so no need to install sepraterly(npm --version)



3.run one command that will make local system as JSON server  ( install json - serve)
                npm install -g json-server

4.go to c:\\ Users\DELL  and then create json file which will contain some data (in my case i have created info.json) just a notpad file saved with .json extension


5.If you have created json file again go back to command prompt and run a command 


             json -server file name  
                 
             Ex; json-server info.json  
    
        (when file will get open copy the resource address and paste it in chrome browser) and hence API is created.

6... 
            1)
            prerequiste: Command prompt should be running and browser too

            2)now apply all the methods of http that is get/post/put/delete and check their responses respectively.(i have created create own api collection)
               
            3)to run the fake api collection all command that is get/post/put/delete together in the runner window drag fake api file to the runner and go to file              >setting>proxy>Add a custtom proxy configuration check it and then change address to 127.0.0.1:3000 and then uncheck it and than run create own api .
