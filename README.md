# Secure ASP.NET Core Web API using JWT Authentication
# What is JWT?
JWT or JSON Web Token is basically a way to format tokens, which represent an encoded structure of data that is compact, url-safe, secure and self-contained.

JWT authentication is a standard way to communicate between APIs and clients, so both parties can make sure that the data being sent/received is trusted and verified.

JWTs should be issued by a server and digitally sign it using a cryptographically secure secret, so that it will make sure that any attacker won’t be able to tamper the payload sent within the token and impersonate the legit user.

JWT structure includes 3 parts, separated with dots, each of which is a base64 url-encoded string and formatted in JSON:
# Header.Payload.Signature

Header: represents the algorithm used to hash the secret (example HMACSHA256)
Payload: the list of data or claims to be transferred between client and api
Signature: the hashing of the concatenation of Header and Payload )

# Let’s create a new Project in Visual Studio 2019.
![image](https://user-images.githubusercontent.com/37914930/125211249-b93e0080-e2ad-11eb-9eed-bb6760e9ceb3.png)
We need to choose ASP.NET Core Web Api Template, then press Create.

Adding Microsoft.EntityFramvorc.Core
![image](https://user-images.githubusercontent.com/37914930/125211276-dd99dd00-e2ad-11eb-9bf2-1ef95308aad4.png)


