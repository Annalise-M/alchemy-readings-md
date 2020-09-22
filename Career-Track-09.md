CT Reading Notes - 09: Express

    Using express routing @ https://expressjs.com/en/guide/routing.html

    Supertest @ https://github.com/visionmedia/supertest

    Using express middleware @ https://expressjs.com/en/guide/using-middleware.html

    Express middleware @ https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm

    Express middleware list @ https://expressjs.com/en/resources/middleware.html

    Bookmarked:
        status codes @ https://www.restapitutorial.com/httpstatuscodes.html

---
    Using express routing: 
        Routing - 
            refers to how an application’s endpoints (URIs) respond to client requests.

        Route methods -
            is derived fromoneof the HTTP methods, and is attached to an instance of the express class. Express supports methods that correspond to all HTTP request methods: get, post, and so on.
        
        Route paths -
            in combination with a request method, define the endpoints at which requests can be made. 
            Route paths can be strings, string patterns, or regular expressions. 

        Route parameters -
            are named URL segments, used to capture the values specified at their position in the URL. (ie. URL search params)
---
    example: 
            Route path: /users/:userId/books/:bookId
            Request URL: http://localhost:3000/users/34/books/8989
            req.params: { "userId": "34", "bookId": "8989" }
---
        Route handlers -
            can provide multiplue callback functions that behave like middleware to handle a request.
            The only exception is that these callbacks might invoke next('route') to bypass the remaining route callbacks.
            Route handlers can be in the form of a function, an array of functions, or combinations of both.

        Response methods -
            the methods on a response object (res from the below example)can send a response to the client, and terminate teh request-response cycle. If none of these methods are called from a route handler, the client request will be left hanging. 

---
    Method	Description
    res.download() - Prompt a file to be downloaded.
    res.end() - End the response process.
    res.json() - Send a JSON response.
    res.jsonp() - Send a JSON response with JSONP support.
    res.redirect() - Redirect a request.
    res.render() - Render a view template.
    res.send() - Send a response of various types.
    res.sendFile() - Send a file as an octet stream.
    res.sendStatus() - Set the response status code and send its string representation as the response body.
---
    app.route() -
        chainable route handlers for a route path by using app.route()
    
    express.Router -
        Use the express.Router class to create modular, mountable route handlers. A Router instance is a complete middleware and routing system; for this reason, it is often referred to as a “mini-app”.

--- 
    Supertest -
        an API that assists in testing Http applications (build upon superagent - another API) that simulates http requests testing your applications response.
        (see link for more details)

---
    Using Express middleware -
        Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

    Express applications can use the following types of middleware:
        Application-level middleware
        Router-level middleware
        Error-handling middleware
        Built-in middleware
        Third-party middleware

    (see link for more details)

---
    ExpressJS - Middleware
        Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. These functions are used to modify req and res objects for tasks like parsing request bodies, adding response headers, etc.
        
        One of the most important things about middleware in Express is the order in which they are written/included in your file; the order in which they are executed, given that the route matches also needs to be considered.
---
    Express middleware list - 
        (see link for detailed list)
