Readings: HTTP and REST

    Read:

        * http basics - https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177

        * How DNS works - https://howdns.works/
---
    Watch: 

        * http and rest (video) - https://www.youtube.com/watch?v=Q-BpqyOT3a8
---
    Bookmark:

        * http reference - https://code-maze.com/the-http-reference/

        * rest reference - https://www.restapitutorial.com/lessons/httpmethods.html

---
    http basics - 
        HTTP stands for Hypertext Transfer Protocol. It's a stateless, application-layer protocol for communicating between distributed systems, and is the foundation of the modern web.
        It allows for communication between a variety of hosts and clients as well as supports a mixture of network configs. 
        Communication usually takes place over TCP/IP (default port is 80- others can still be used).
        Communication is based off of the request/response pair. 
        Client initiates HTTP request which is served with a HTTP response (thing URL address translating computer guts into words for the user).

    URLs -
        the heart of web communications is the request message, which are sent via Uniform Resource Locators (URLs).

    Verbs -
        These request verbs are:

            GET: fetch an existing resource. The URL contains all the necessary information the server needs to locate and return the resource.

            POST: create a new resource. POST requests usually carry a payload that specifies the data for the new resource.

            PUT: update an existing resource. The payload may contain the updated data for the resource.

            DELETE: delete an existing resource.
    
            There are some lesser used verbs that HTTP also supports:

            HEAD: this is similar to GET, but without the message body. It's used to retrieve the server headers for a particular resource, generally to check if the resource has changed, via timestamps.

            TRACE: used to retrieve the hops that a request takes to round trip from the server. Each intermediate proxy or gateway would inject its IP or DNS name into the Via header field. This can be used for diagnostic purposes.

            OPTIONS: used to retrieve the server capabilities. On the client-side, it can be used to modify the request based on what the server can support.

    Status codes and error messages (see website link).
    General Headers
        There are a few headers (general headers) that are shared by both request and response messages:

            general-header = Cache-Control            
                            | Connection        
                            | Date              
                            | Pragma            
                            | Trailer           
                            | Transfer-Encoding 
                            | Upgrade           
                            | Via               
                            | Warning

    Entity headers - 
        Request and Response messages may also include entity headers to provide meta-information about the the content (aka Message Body or Entity).

            entity-header  = Allow                    
               | Content-Encoding  
               | Content-Language  
               | Content-Length    
               | Content-Location  
               | Content-MD5       
               | Content-Range     
               | Content-Type      
               | Expires           
               | Last-Modified
    
    Request formats (see link for more info).
---

    How DSN works
        - a cute online comic that goes through the process and explanation of how DSN works. 
        (see link for more info)
---

    http and rest - watched 
        - same info (see link for more)
---

    Bookmarks are linked at the top. 
