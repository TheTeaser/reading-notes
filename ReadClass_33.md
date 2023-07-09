# Reading Topics #33:  Authentication & Production Server

## JWTs:

he primary purpose of JSON Web Tokens (JWTs) is to securely transmit information between parties as a compact and self-contained format. JWTs are often used for authentication and authorization purposes in web applications and APIs.

Here's how they work in terms of encoding and decoding data:

1. Encoding:

    - The header contains metadata about the type of token (JWT) and the hashing algorithm used to generate the signature. It is encoded as a Base64Url string.
    - The payload, also known as the claims, contains the actual data and additional information about the token, such as the user's ID, roles, and expiration time. It is also encoded as a Base64Url string.
    - The signature is generated by taking the encoded header, encoded payload, and a secret key, and hashing them together using the specified algorithm in the header. The signature provides integrity and ensures that the token hasn't been tampered with.
    - The encoded header, encoded payload, and signature are concatenated together with periods ('.') as separators to form the complete JWT.
2. Decoding:

    - To decode a JWT, the receiving party needs to extract the header, payload, and signature from the token. This is done by splitting the JWT string at the periods ('.') to obtain the three components.
    - The header and payload are then Base64Url decoded to retrieve the original JSON data.
    - The signature is typically used to verify the authenticity of the token. The receiving party performs the same hashing algorithm on the decoded header and payload, along with the secret key (which should be securely stored), and compares the resulting signature with the received signature

---

## JWT Authentication integrate with Django REST:

The key components involved in this process are:

1. Installation and Configuration:

- Install the required packages, such as djangorestframework and djangorestframework_simplejwt, which provides JWT support for DRF.
Configure the authentication settings in your Django project's settings.py file, including specifying the authentication class and token expiration settings.
2. User Authentication and Token Generation:

- When a user successfully authenticates (e.g., by providing valid credentials), generate a JWT token for that user using the djangorestframework_simplejwt library.
Typically, the token generation occurs within a login view or authentication endpoint. The library generates a JWT containing the user's ID or other identifying information.
3. Token Verification and Authentication:

- For protected API endpoints, use the rest_framework_simplejwt.authentication.JWTAuthentication class as the authentication class in the DRF settings.
When a request is made to an API endpoint, the JWTAuthentication class verifies and extracts the JWT token from the request headers.
The library verifies the token's integrity, expiration, and other claims. If the token is valid, the associated user is considered authenticated, and the request proceeds.
4. Applying Authentication to API Endpoints:

- In your DRF views or viewsets, apply the authentication_classes decorator or property to specify JWT authentication for the desired endpoints.
You can also use the permission_classes decorator or property to define specific permissions (e.g., IsAuthenticated) for authenticated users.

---

## Django server alternatives:

Django's built-in runserver is not suitable for production environments due to the following reasons:

1. Performance and Scalability: The runserver is designed for development purposes and is not optimized for handling high traffic or heavy loads.

2. Security: The runserver is not intended to be used in a publicly accessible environment.

3. Stability and Reliability: The runserver is not designed to handle long-running processes or to automatically restart on failures.

For deploying a Django application in a production environment, it is recommended to consider alternative server options, such as:

- Gunicorn (Green Unicorn): Gunicorn is a widely used Python WSGI HTTP server.

- uWSGI: uWSGI is another popular option for deploying Django applications. 

- Nginx + uWSGI or Gunicorn: Nginx is a powerful web server and reverse proxy server. 
---