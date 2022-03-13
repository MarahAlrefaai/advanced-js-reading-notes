What header(s) are used in authentication and authorization

Basic Auth
Bearer Token
API Key
Digest Auth
OAuth 2.0
Hawk Authentication
AWS Signature

What is safe to put into a JWT
When we want to signature a new Json web token; it is better to use a unique field from the user's record in the database along with a secret key that is not revealed to the public, it is also recommended to avoid using the password to generate the token, so we can use either the username or email as long as they are unique fields along with the secret key.

How are JWTs validated
The rule of thumb is - you should always validate an incoming JWT. You should do it, even if you're working on an internal network - where the Authorization Server, the Client and the Resource Server aren't connected through the Internet. You shouldn't rely on your environment settings to be part of your security scheme. If you move your services to a public domain, the threat model will change and you will have to remember to update your security measures - experience shows that this is very often overlooked. Moreover, implementing token validation from the start will guard your from situations where someone manages to break into your network, or you would have a malicious actor in your organization.

The one case when you could consider omitting checking the signature of the token is when you first get it in the response from the token endpoint of the Authorization Server using TLS. You should definitely validate a token if using the implicit flow, and the token is sent back to the client by means of a redirect URI, as in such case there is a greater risk of someone tampering with the token before you manage to retrieve it.