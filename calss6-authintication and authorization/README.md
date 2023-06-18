# Authintication and authorization

 *Explain to a non-technical friend how you would safely hash and store a password.*


To safely hash and store a password, the system transforms the password into a unique string of characters using a one-way hashing process. The hashed password, along with a random salt, is stored in the system. Hashing makes it virtually impossible to reverse-engineer the original password from the stored hash. When logging in, the entered password is hashed and compared with the stored hash. By employing hashing and salting techniques, passwords are securely protected even if the stored hashes are compromised, ensuring the safety of user accounts.


*What is Bcrypt?*


Bcrypt is a widely used cryptographic hashing function specifically designed for securely storing passwords. It is an algorithm that takes a password as input and applies a salted hashing process, which includes multiple iterations and a built-in random salt. Bcrypt is known for its ability to slow down hashing computations, making it resistant to brute-force attacks. Its design aims to protect against password cracking techniques and ensure the confidentiality of user passwords by producing a unique and irreversible hash for each input. Bcrypt is commonly utilized in web applications and systems to enhance password security.

*Why might you use something like Bcrypt?*


Bcrypt is used for secure password hashing and storage due to its slow and computationally expensive nature, protection against rainbow table attacks, wide support across different platforms, and future-proofing capabilities. It enhances password security by making it difficult for attackers to crack passwords and ensures consistent protection across various systems and frameworks.

<hr>

*What is Basic Authentication?*

Basic Authentication is a simple method for implementing user authentication in web-based applications or APIs. It involves sending the username and password credentials encoded in Base64 format with each request. The server validates these credentials against a user database and grants access if they match. However, Basic Authentication has security limitations, such as the lack of encryption, making it susceptible to interception and replay attacks. Therefore, it is typically recommended to use more secure authentication mechanisms, such as token-based authentication or OAuth, when transmitting sensitive data over the internet.

*What properties are necessary in the header of a Basic Auth request?*

In a Basic Auth request, the necessary property in the header is "Authorization", which includes the authentication scheme ("Basic") and the Base64-encoded credentials of the form "username:password".

*How are username:password in Basic Auth encoded?*


n Basic Authentication, the username:password combination is encoded using Base64 encoding. Base64 encoding converts binary or text data into ASCII characters to ensure safe transmission in a text-based protocol. The username and password are combined in the format "username:password" and then Base64-encoded as a single string. This encoded string is included in the Authorization header of the HTTP request.

<hr>

*Define the authentication process to a non-technical recruiter.*

Authentication is the process of verifying and confirming the identity of an individual or user in a system. It is a crucial step in ensuring that the right people have access to the appropriate resources and information. When a user wants to access a system or platform, they are required to provide certain credentials, such as a username and password. These credentials act as proof of their identity. The system then checks the provided credentials against a stored record to validate if they are correct. If the credentials match, the user is granted access to the system. Authentication helps protect sensitive data and ensures that only authorized individuals can access specific areas or perform certain actions within the system. It is an essential aspect of maintaining security and privacy in modern digital environments.

*How should your error messaging respond (both HTTP and HTML)? Why?*

Clear and informative error messages are important in both the HTTP response and HTML content. HTTP status codes indicate the nature of the error, while user-friendly error messages in the HTML help users understand and address the problem. This improves troubleshooting, user experience, and problem resolution.











