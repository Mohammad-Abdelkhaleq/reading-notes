### Code 401 - *Class 2 readings *

#### JWT

What is a JSON Web Token (JWT)?

A JSON Web Token (JWT) is a compact and secure way of representing claims or information between two parties. It is commonly used for authentication and authorization in web applications. It consists of three parts: a header, a payload, and a signature. The header specifies the token type and signing algorithm, while the payload contains the claims or user information. The signature is used to verify the integrity of the token. JWTs are self-contained and can be easily transmitted as strings, making them efficient for stateless authentication.

When should we use JSON Web Tokens?

JSON Web Tokens (JWTs) are used for authentication, single sign-on, authorization, and information exchange. They are suitable for stateless authentication, enabling secure transmission of data between different systems. JWTs are especially useful in mobile and cross-domain applications.


Claims are expected in which structural component of a JWT?


Claims are expected in the payload component of a JSON Web Token (JWT). The payload is where the claims or information about the user or entity being authenticated are stored. Claims can include various attributes such as user identifiers, roles, permissions, expiration time, and other relevant data. The payload is encoded and included as the middle part of the JWT, between the header and the signature. When the JWT is decoded, the claims can be extracted and used for authentication, authorization, or other purposes in the application.

<hr>

If I get a JWT and I can decode the payload, how can we call that secure?


JWTs are considered secure due to the use of signatures to verify integrity and the secure transmission of tokens. While the payload can be decoded, sensitive information should not be included. Token expiration and revocation mechanisms further enhance security.

If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.


Both the sender and receiver of a JSON Web Token (JWT) must know the shared secret key that is used to create the signature. This key is appended during the signature creation process and is crucial for verifying the authenticity and integrity of the token. Safely managing and protecting the shared secret key is essential for the security of the JWT-based system.

Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

Imagine you have a locked box with two compartments: one for the content and another for a key. The content represents the data you want to send, and the key represents the secret. You securely send the locked box to the recipient, who retrieves the key from a trusted source to unlock the box and access the content. Emphasize the importance of keeping the key secure and not sharing it with unauthorized individuals.

<hr>

Why use JWT?


JWTs are used because they enable stateless authentication, support single sign-on (SSO), provide security through digital signatures, offer flexibility and extensibility with custom claims, and ensure interoperability across different systems and technologies. They are widely adopted for their efficiency, scalability, and ability to work in decentralized architectures.

JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.


JWT being compact and self-contained means that all necessary information is included within the token itself. This makes it easy to handle and transmit without the need for additional data storage or complex configurations. It simplifies authentication and authorization processes for non-technical individuals by keeping everything in one simple package.

The three components of a JWT signature are:

- Header: Contains the token type and signing algorithm.

- Payload: Holds the claims or information about the user or entity.

- Signature: Ensures the integrity and authenticity of the token.
