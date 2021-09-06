## What is REST?

In 2000, Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

A primary advantage of REST over HTTP is that it uses open standards, and does not bind the implementation of the API or the client applications to any specific implementation. For example, a REST web service could be written in ASP.NET, and client applications can use any language or toolset that can generate HTTP requests and parse HTTP responses.

### Organize the API design around resources

Focus on the business entities that the web API exposes. For example, in an e-commerce system, the primary entities might be customers and orders. Creating an order can be achieved by sending an HTTP POST request that contains the order information. The HTTP response indicates whether the order was placed successfully or not. When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource). 

```
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid

```

### Define API operations in terms of HTTP methods

The HTTP protocol defines a number of methods that assign semantic meaning to a request. The common HTTP methods used by most RESTful web APIs are:

GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
* POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that 
* POST can also be used to trigger operations that don't actually create resources.
* PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
DELETE removes the resource at the specified URI.