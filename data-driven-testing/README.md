- data driven testing
------------------

- how to run collections
- import/export the collections

Req URL(post):http://dummy.restapiexample.com/api/v1/create

Request Body/request Payload


{"name":"santosh",
    "salary":"100",
    "age":"40"}
Data Format:csv/json

//request body format for extracting data externally


{
    "name":"{{name}}",
    "salary":"{{salary}}",
    "age":"{{age}}"
    }


//we can covert csv into json and vice versa on online platform


https://csvjson.com/csv2json

