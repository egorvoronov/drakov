FORMAT: 1A

# Return all the things
Lists all the things from the API

## Things [/headers]

### Retrieve a dummy object [GET]
Check Authorization header

+ Request

    + Headers

        Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

+ Response 200

+ Request

    + Headers

        Authorization: Basic foo

+ Response 401


## Things [/things]

### Retrieve all the things with no header [GET]
+ Request JSON Message
            
+ Response 200 (application/json;charset=UTF-8)

    + Body

           {
              "header":"absent"
            }
            


### Retrieve all the things with specific header [GET]
+ Request JSON Message
    
    + Headers

            content-type: application/json

            
+ Response 200 

    + Headers

            content-type: application/json;charset=UTF-8

    + Body

            {
                 "header":"json"
           }
