# API Design Best Practices


## Reading questions :

1. What does REST stand for?

    It stands for Representational State Transfer
2. REST APIs are designed around a **resource**.


3. What is an identifer of a resource? Give an example.

    >web site for example: https://adventure-works.com/orders/1
4. What are the most common HTTP verbs?

    * GET
    * POST
    * PUT
    * PATCH
    * DELETE
5. What should the URIs be based on?

    they are recommend to be based on nouns and not verbs.
6. Give an example of a good URI.

    > good example on a good URI: https://adventure-works.com/orders
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

    it mean that our web API will be expose to a large number of small resources.
8. What status code does a successful GET request return?

    it would typically returns HTTP status code 200 (OK).
9. What status code does an unsuccessful GET request return?

    if not the method should return 404 (Not Found).
10. What status code does a successful POST request return?

    it will returns HTTP status code 201 (Created).
11. What status code does a successful DELETE request return?
    it will return HTTP status code 204 (No Content) with no response body.

