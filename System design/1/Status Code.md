***Definition***

A status code is a numerical code that is sent by a server in response to a client's request made to a web server. It provides information about the status of the request and indicates whether it was successful, encountered an error, or requires further action. Status codes are a crucial part of the HTTP protocol, defining the outcome of each HTTP request-response cycle. They are grouped into different categories, each representing a specific type of response.

Here are some common categories of HTTP status codes along with their meanings:

***1xx - Informational:*** 

These status codes indicate that the request has been received and the process is continuing. They are primarily used for informational purposes and rarely encountered in practice.

***2xx - Success:*** 

These status codes indicate that the request was successfully received, understood, and processed by the server.

- **200 OK:** The request has succeeded.
- **201 Created:** The request has been fulfilled and a new resource has been created.
- **204 No Content:** The server successfully processed the request but there is no content to return.

***3xx - Redirection:*** 

These status codes indicate that further action needs to be taken by the client to complete the request.

- **301 Moved Permanently:** The requested resource has been permanently moved to a new location.
- **302 Found (or Moved Temporarily):** The requested resource has been temporarily moved to a different location.
- **304 Not Modified:** The client's cached copy of the requested resource is still valid and can be used.

***4xx - Client Error:*** 

These status codes indicate that there was an error in the client's request, such as invalid syntax or insufficient permissions.

- **400 Bad Request:** The server could not understand the request due to invalid syntax.
- **401 Unauthorized:** The request requires user authentication.
- **404 Not Found:** The requested resource could not be found on the server.

***5xx - Server Error:*** 

These status codes indicate that the server encountered an error while processing the request.

- **500 Internal Server Error:** A generic error message indicating that something went wrong on the server.
- **503 Service Unavailable:** The server is currently unable to handle the request due to temporary overloading or maintenance.