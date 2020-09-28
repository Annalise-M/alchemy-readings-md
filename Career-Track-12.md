CT Class 12 Reading notes:

<a href="https://medium.com/@danboterhoven/why-you-should-use-bcrypt-to-hash-passwords-af330100b861">Why you should use bcrypt</a>

<a href="https://auth0.com/blog/hashing-in-action-understanding-bcrypt/">Understanding bcrypt</a>

<a href="https://auth0.com/docs/security/store-tokens">Where to store JWT</a>

___
    Why you should use bcrypt
        - Hashed password solutions fall short
        - Plain text passwords
        - One way hash
        - 'Salting' the password
        - Random 'salt' for each user
        
        - the BCrypt Solution (the BCrypt hashing function — designed by Niels Provos and David Mazières in 1999.)
        - BCrypt is based on the Blowfish block cipher cryptomatic algorithm and takes the form of an adaptive hash function. 
            Using a Key Factor, BCrypt is able to adjust the cost of hashing. With Key Factor changes, the hash output can be influenced. In this way, BCrypt remains extremely resistant to hacks, especially a type of password cracking called rainbow table.
        This Key Factor will continue to be a key feature as computers become more powerful in the future, because it compensates for these powerful computers and slows down hashing speed significantly. Ultimately slowing down the cracking process until it’s no longer a viable strategy.
        (for more info. see link above)
---
    Understanding bcrypt -
        At Auth0, the integrity and security of our data are one of our highest priorities. We use the industry-grade and battle-tested bcrypt algorithm to securely hash and salt passwords. bcrypt allows building a password security platform that can evolve alongside hardware technology to guard against the threats that the future may bring, such as attackers having the computing power to crack passwords twice as fast. 

        bcrypt was designed by Niels Provos and David Mazières based on the Blowfish cipher: b for Blowfish and crypt for the name of the hashing function used by the UNIX password system.
        (for more info. see link above)
---
    Token Storage -
        Next.js static site scenarios
    When you're building a Next.js application, authentication might be needed in the following cases:

    When accessing a page

    When accessing an API route

    When your application calls an API hosted outside of your Next.js application on behalf of the user

    Where a server is available, your app can handle the interaction with Auth0 and create a session, but in this model, we don't have a backend. All of the work happens on the frontend:

    The user is redirected to Auth0.

    When the user is successfully signed in, they will be redirected back to the application.

    The client-side will complete the code exchange with Auth0 and retrieve the user's id_token and access_token which will be stored in memory.

        (for more info. see link above)

        