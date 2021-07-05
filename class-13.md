In your own words, describe what each group of status code represents:
100’s = These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.


200’s =These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.


300’s =These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.


400’s =These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.
500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.


What is a status code 202?

202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.


What is a status code 308?

303 See Other - Like the 202 code but using a Location header field in response to informing the client about the location of the created resource or an endpoint that lets the client check for the status of the creation process. Some clients follow the status codes of the Redirect-class automatically. This code is usually only used for POST requests.



What code would you use if an update didn’t return data to a client?

204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

What code would you use if a resource used to exist but no longer does?

410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

What is the ‘Forbidden’ status code?

403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.





Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

Why do we need to pull our MongoDB database string out of our server and put it into our .env?
What is middleware?
Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system. ... Middleware helps developers build applications more efficiently. It acts like the connective tissue between applications, data, and users.

What does app.use(express.json()) do?
express. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app.

What does the /:id mean in a route?
Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.

What is the difference beween PUT and PATCH?
The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.


How do you make a defalut value in a schema?
Make mongoose string schema type default value as blank and make the field optional. testschema = mongoose. 
            Schema({ name:{ type:String, required:true, unique:true }, image:{ type:String, required:true }, category:{ type:String }, });

What does a 500 error status code mean?
The HyperText Transfer Protocol (HTTP) 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. This error response is a generic "catch-all" response

What is the difference between a status 200 and a status 201?

The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).

