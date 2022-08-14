# JSON Web Tokens

- JSON Web Token (JWT) is an open standard that defines a compact and self-contained way for securing transmitting info between parites as a JSON object. 
- The info can be verified and trusted becuase it is digitally signed.
- JWTs can be signed using a secret (with the HMAC algo) or a public/private key pair using RSA or ECDSA.
- Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parites.

## When should you use JSON Web Tokens?

- Authorization: Most common scenario. Once user is logged in, each subsequent request will includ the JWT, allowing the user to access routhes, services and resources that are permitted with that token.
- Information Exchange: JWT are a good way of securely transmitting info between parties. Since JWT c an be signed, you can be sure the senders are who they say they are and also the content hasn't been tampered with.

### What is the JSON Web Token structure?

- JWT consist of three parts separated by ( . )
- Header, Payload and Signature.
- JWT look something like this: xxxx.yyyy.zzzzz

#### Header

- consist of two parts: type of token and signing algo being used, such as HMAC, SHA256 or RSA.

#### Payload

- Payload contains Claims. Claims are statements about an entity (the user) and additional data.
- There are three tyups od claims: registered, public and private claims.
- Registered claims: not mandatory but recommended, iss(issuer), exp(expiration time), sub(subject), aud(audience)
- Public: can be defined at will by those using JWTs. To avoid collisions they shjould be defined in the IANA JSON Web Token Registry or be defined as a URI that contains resitant namespace.
- Private: custom claims created to shre information between parties that agree on using them and are neither registered or public claims.

#### Signature

- to create a signature part you have to take the encoded header, the encoded payload, a secret, the algo specified in the header, and sign that.
- signature is used to verify the message wasn't changed along the way, also verifies the sender of the JWT.

### How do JWTs work?

- when users log in using their credentials, a JWT will be returned.
- Should not keep tokens longer than required.
- whenever user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema.
