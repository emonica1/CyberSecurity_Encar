HTTP Requests and Responses
Answer the following questions about the HTTP request and response process.


What type of architecture does the HTTP request and response process occur in?

        Client Server Architecture and the requests are made from the client, to the server, and then back to the client.

What are the different parts of an HTTP request?

        The different parts of an HTTP request are request line, request header, and request body.


Which part of an HTTP request is optional?

        The request body is optional.


What are the three parts of an HTTP response?

        Status line, header, and body.


Which number class of status codes represents errors?

        [400..499] :: Client errors && [500..599] :: Server errors

What are the two most common request methods that a security professional will encounter?

    GET and POST


Which type of HTTP request method is used for sending data?

        POST


Which part of an HTTP request contains the data being sent to the server?

        BODY


In which part of an HTTP response does the browser receive the web code to generate and style a web page?

        BODY

Using curl
Answer the following questions about curl:


What are the advantages of using curl over the browser?

        It has the ability to manage HTTP Requests / responses in a repeatable , programmatic way, quickly test HTTP HTTP Requests in away that can be automated, and supports numerous protocols even if a UI is not present
        


Which curl option is used to change the request method?

        curl -X




Which curl option is used to set request headers?

        curl -H


Which curl option is used to view the response header?

        curl -i


Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?

        GET

Recall that HTTP servers need to be able to recognize clients from one another. They do this through sessions and cookies.
Answer the following questions about sessions and cookies:


Which response header sends a cookie to the client?

HTTP/1.1 200 OK
Content-type: text/html
Set-Cookie: cart=Bob

        Set-Cookie sends cookie to the client.



Which request header will continue the client's session?

GET /cart HTTP/1.1
Host: www.example.org
Cookie: cart=Bob

        The Cookie will save/continue the client's session




Example HTTP Requests and Responses
Look through the following example HTTP request and response and answer the following questions:
HTTP Request

POST /login.php HTTP/1.1
Host: example.com
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
Content-Type: application/x-www-form-urlencoded
Content-Length: 34
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Mobile Safari/537.36

username=Barbara&password=password




What is the request method?

        HTTP defines a set of request methods to indicate the desired action to be performed for a given resource. In this case, the request method is POST       

Which header expresses the client's preference for an encrypted response?

        HTTP Upgrade-Insecure-Requests request header


Does the request have a user session associated with it?

        No



What kind of data is being sent from this request body?

        Login Credentials 


HTTP Response

HTTP/1.1 200 OK
Date: Mon, 16 Mar 2020 17:05:43 GMT
Last-Modified: Sat, 01 Feb 2020 00:00:00 GMT
Content-Encoding: gzip
Expires: Fri, 01 May 2020 00:00:00 GMT
Server: Apache
Set-Cookie: SessionID=5
Content-Type: text/html; charset=UTF-8
Strict-Transport-Security: max-age=31536000; includeSubDomains
X-Content-Type: NoSniff
X-Frame-Options: DENY
X-XSS-Protection: 1; mode=block

[page content]




What is the response status code?

        CC


What web server is handling this HTTP response?

        Apache webserver 


Does this response have a user session associated to it?

        Yes, SessionID=5


What kind of content is likely to be in the [page content] response body?

        Details of the page configuration 


If your class covered security headers, what security request headers have been included?

        Strict transport security, oe XSS protection.



Monoliths and Microservices
Answer the following questions about monoliths and microservices:


What are the individual components of microservices called?

        Services


What is a service that writes to a database and communicates to other services?

        APIs


What type of underlying technology allows for microservices to become scalable and have redundancy?

        Load Plancer or Containers



Deploying and Testing a Container Set
Answer the following questions about multi-container deployment:


What tool can be used to deploy multiple containers at once?

        Docker


What kind of file format is required for us to deploy a container set?

        .yml format


Databases


Which type of SQL query would we use to see all of the information within a table called customers?

        Select Column & From Customers

Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)

        INSERT INTO [columns] VALUES [values]

Why would we never run DELETE FROM <table-name>; by itself?
     
        It'll delete the entire table because there is no select statement  


