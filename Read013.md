# Reading questions:

## Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:

        100’s = they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.
        200’s = They tell the client that its request was accepted.
        300’s = They tell the client that the resource they are requesting isn’t available at the expected location anymore.
        400’s = They are all about invalid requests a client sent to a server. 
        500’s = Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server.

2. What is a status code 202? 
    
    asynchronous processing of a request

3. What is a status code 308?

    Permanent Redirec

4. What code would you use if an update didn’t return data to a client?

    204 No Content

5. What code would you use if a resource used to exist but no longer does?

    410 Gone

6. What is the ‘Forbidden’ status code? 

    403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.