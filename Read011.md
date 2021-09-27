# Reading questions:

## What is OAuth

1. What is OAuth?

    >is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

2. Give an example of what using OAuth would look like.

    One of the most common ways you see now is when you install a game and you open it for the first time it will tell you you can login using facebook, google..etc which will connect your account to the game.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    1. The sites connect using Oauth on behalf of the user after he provide identification.
    2. The sites create this one time token and a one time secret unique for the websites involved.
    3. The first site gives this token and secret to the initiating user’s client software.
    4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    6. The user approves (or their software silently approves) a particular transaction type at the first website.
    7. The user is given an approved access token (notice it’s no longer a request token).
    8. The user gives the approved access token to the first website.
    9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
    10. The second website lets the first website access their site on behalf of the user.
    11. The user sees a successfully completed transaction occurring.

4. What is OpenID?

    was one of the first means for logging into the then-popular LiveJournal blogging site but quickly spread to other sites.

## Authorization and Authentication flows

1. What is the difference between authorization and authentication?

    authorization gives access users and get the protected resources with some sort of key or ID  while Authentication is about confirming the identity of the user.

2. What is Authorization Code Flow?

    Is using the access key token to obtain authorization for API requests.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    Is a process used to authenticate the user and verify them.

4. What is Implicit Flow with Form Post?

    Is used to implement sign ins in the website.

5. What is Client Credentials Flow?

    Is used to authorize when you call your protected APIs .

6. What is Device Authorization Flow?

    The device asks the user to go to a link on their computer or smartphone and authorize the device.

7. What is Resource Owner Password Flow?

    (Not recommended)

    > requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information.