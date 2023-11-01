# Spring-Security-JWT
How to secure your Spring Boot REST APIs with JSON Web Tokens

# How to Run

1- Clone the project repository from Git (if it's not already cloned).

2- Import the project into your favorite Java IDE (e.g., IntelliJ, Eclipse, etc.).

3- create public key and private key 
```code
# create rsa key pair
openssl genrsa -out keypair.pem 2048
# extract public key
openssl rsa -in keypair.pem -pubout -out public.pem
# create private key in PKCS#8 format
openssl pkcs8 -topk8 -inform PEM -outform PEM -nocrypt -in keypair.pem -out private.pem
```

4- Build the project to resolve dependencies.
