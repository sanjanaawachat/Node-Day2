node
========Day2==================================================

1. What are the different types of HTTP requests?

ans:
Hypertext Transfer Protocol (HTTP) defines a variety of request methods to describe what action is to be done on a certain resource. The most often used HTTP request methods are GET, POST, PUT, PATCH, and DELETE.


Let’s understand the use cases of HTTP requests:

GET:
 A GET request reads or retrieves data from a web server. If the data is correctly collected from the server, the HTTP status code is 200 (OK).

POST:
 A POST request is used to transmit data to the server. It produces an HTTP status code of 201 on successful creation.

PUT:
 A PUT request is used to alter server data. It replaces all of the content at a specific position with data from the body payload. It will generate one if there are no resources that match the request.

PATCH:
 A PATCH request is identical to a PUT request, with the exception that it alters a portion of the data.

DELETE: 
A DELETE request is used to delete data from a specific place on the server.

=================================================================
2.Explain the concept of middleware in Node.js.
ans:

Express.js is a routing and Middleware framework for handling the different routing of the webpage and it works between the request and response cycle. Middleware gets executed after the server receives the request and before the controller actions send the response. Middleware has the access to the request object, responses object, and next, it can process the request before the server send a response. An Express-based application is a series of middleware function calls.
 
Middleware working

Advantages of using middleware:

Middleware can process request objects multiple times before the server works for that request.
Middleware can be used to add logging and authentication functionality.
Middleware improves client-side rendering performance.
Middleware is used for setting some specific HTTP headers.
Middleware helps for Optimization and better performance.
Middleware Chaining: Middleware can be chained from one to another, Hence creating a chain of functions that are executed in order. The last function sends the response back to the browser. So, before sending the response back to the browser the different middleware process the request.
==================================================================
3.Explain CORS

ans:
Cross-origin resource sharing (CORS) is a browser mechanism which enables controlled access to resources located outside of a given domain. It extends and adds flexibility to the same-origin policy (SOP). However, it also provides potential for cross-domain attacks, if a website's CORS policy is poorly configured and implemented. CORS is not a protection against cross-origin attacks such as cross-site request forgery (CSRF).

==================================================================
4.What is Express. how it helps you to create a backend application

ans:
Express is a small framework that sits on top of Node.js’s web server functionality to simplify its APIs and add helpful new features.It makes it easier to organize your application’s functionality with middle ware and routing; it adds helpful utilities to Node.js’s HTTP objects;it facilitates the rendering of dynamic HTTP objects.

Express is a part of MEAN stack, a full stack JavaScript solution used in building fast, robust, and maintainable production web applications.

==================================================================
5.Explain min 5 status codes gets used in Backend development

1.100 Information
The HTTP 100 informational status response code indicates that everything is OK and that the client can continue with the request.
Other informational codes:

100 — Continue;
101 — Switching protocol;
103 — Checkpoints.

2.200 Successful
The HTTP 200 success status response code indicates that the request has succeeded. A 200 response is cacheable by default.

The meaning of success depends on the HTTP request method:

GET: The resource has been fetched and is sent in the message body.
HEAD: The representation headers are included in the response without a body message.
POST: The resource describing the result of the action is sent in the message body
TRACE: The body contains the request message as received by the server.

The successful result of a PUT or a DELETE is often not a 200 OK but a 204 No Content (or a 201 Created when the resource is uploaded for the first time).


3.300 Redirection
The HTTP 300 redirect status response code indicates that the request has more than one possible response. The user-agent or the user should choose one of them. As there is no standardized way of choosing one of the responses, this response code is very rarely used.

Redirection types:

301 — Moved Permanently;
302 — Found;
304 — Not Modified;
305 — Use Proxy;
307 — Temporary Redirect.

4.400 Client Errors
The HTTP (HyperText Transfer Protocol) 400 Bad Request response status code indicates that the server cannot or will not process the request due to something that is perceived to be a client error (e.g., malformed request syntax, invalid request message framing, or deceptive request routing).


Other client errors codes:

400: Bad Request;
401: Unauthorized;
403: Forbidden;
404: Not Found;
408: Request Timeout;
410: Gone;
418: A teapot;
429: Too Many Requests.

5.500 Server Errors
The HTTP 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.

This error response is a generic “catch-all” response. Usually, this indicates the server cannot find a better 500 error code to respond. Sometimes, server administrators log error responses like the 500 status code with more details about the request to prevent the error from happening again in the future.


Other server error codes:

500 — Internal Server Error;
502 — Bad Gateway;
503 — Service Unavailable;
504 — Gateway Timeout.

=================================================================
6.Difference between HTTP and HTTPS


1]HTTP stands for HyperText Transfer Protocol and HTTPS stands for HyperText Transfer Protocol Secure.

2]In HTTP, URL begins with “http://” whereas URL starts with “https://”

3]HTTP uses port number 80 for communication and HTTPS uses 443

4]HTTP is considered to be insecure and HTTPS is secure

5]HTTP Works at Application Layer and HTTPS works at Transport Layer

6]In HTTP, Encryption is absent and Encryption is present in HTTPS as discussed above

7]HTTP does not require any certificates and HTTPS needs SSL Certificates

8]HTTP speed is faster than HTTPS and HTTPS speed is slower than HTTP

9]HTTP does not improve search ranking while HTTPS improves search ranking.

10]HTTP does not use data hashtags to secure data, while HTTPS will have the data before sending it and return it to its original state on the receiver side.

****************************************************************