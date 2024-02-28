
***Definition:***

#HTTP stands for Hypertext Transfer Protocol. It is an application-layer protocol used for transmitting hypermedia documents, such as HTML files, over the World Wide Web.

Here are some key points about #HTTP:

***Client-Server Protocol:*** 

#HTTP is a client-server protocol, meaning that requests are initiated by the client (e.g., a web browser) and sent to a server (e.g., a web server), which processes the request and sends back a response.

***Stateless Protocol:*** 

#HTTP is stateless, meaning that each request from a client to a server is independent and not related to any previous requests. This simplifies implementation but requires additional mechanisms (e.g., cookies, session management) for maintaining stateful interactions.

***Request-Response Model:***

#HTTP follows a request-response model, where the client sends a request message to the server, specifying the desired action (e.g., retrieving a webpage), and the server responds with a message containing the requested resource (e.g., the webpage) or an indication of an error.

***Text-based Protocol:*** 

#HTTP messages (requests and responses) are text-based, consisting of a header section followed by an optional message body. The header contains metadata about the message, such as the #HTTP method (e.g., GET, POST), [[Status Code]], [[Content Type]], and other parameters.

***Connectionless:*** 

#HTTP is connectionless, meaning that each request-response cycle occurs within its own connection, and the connection is closed after the response is sent. However, persistent connections (HTTP/1.1) can be used to reuse connections for multiple requests, reducing latency and overhead.

***HTTP Methods:** *

#HTTP defines various methods (e.g., GET, POST, PUT, DELETE) that specify the action to be performed on a resource. The most commonly used methods are GET (retrieve a resource), POST (submit data to be processed), PUT (create or update a resource), and DELETE (remove a resource).

***URLs (Uniform Resource Locators):*** 

Resources on the web are identified by URLs, which specify the location and name of the resource. #HTTP requests include the URL of the requested resource, allowing the server to locate and retrieve the resource.