# Research report login

Francois Haan

# Version control

| Version | Changes | Date |
| --- | --- | --- |
| 1.0 | 1st version | 17/3/2022 |
| 1.1 | Changes to main – question and sub questions | 31/3/2022 |
| 1.2 | conclusion and sources added | 1/4/2022 |
| 1.3 | Added research about jwt&#39;s | 21/4/2022 |
| 1.4 | Changed some headers based on feedback | 30/5/2022 |
| 1.5 | Added apa style sources | 1/6/2022 |

Contents

**[Version control](#_heading=h.gjdgxs) 2**

**[Method](#_heading=h.30j0zll) 4**

**[Problem definition](#_heading=h.58f4dt9wm7af) 5**

**[Main question](#_heading=h.1fob9te) 6**

[How do you use an identity provider?](#_heading=h.tlcrf454xiyx) 6

[Sub questions](#_heading=h.3znysh7) 6

[What is an Identity provider?](#_heading=h.gx1rk8koliv2) 6

[What are the advantages of using an identity provider for security?](#_heading=h.gq96mthp20h3) 6

[What are some of the most popular providers?](#_heading=h.6lgsbtkie9bs) 6

[What is oAuth2?](#_heading=h.5p9jzi38jlh) 6

[How does oAuth2 work](#_heading=h.e0c5h62klwfx) 6

[What is a jwt token?](#_heading=h.h7s2rlq2dhc) 7

[When should i use a web token?](#_heading=h.b501tpysyaj4) 7

[What is a json web token structure?](#_heading=h.118f4t3zf0jo) 7

[How do JSON web tokens work?](#_heading=h.qqmqj8cxsxvs) 8

[Conclusion](#_heading=h.2et92p0) **9**

**[Sources](#_heading=h.zb95378mpm3s) 10**

# Method

I will be using the dot framework: library research and literature study

# Problem definition

The project requires people to be able to login in order to leave a review. In this research report I am going to research the different ways in which to enable users to login, and how secure each method is.

# Main question

### How do you use an identity provider?

## Sub questions

### What is an Identity provider?

An identity provider is a system that creates, maintains and manages information and provides authentication. examples of such services are github, facebook, google and many more.

Lutkevich, B. (2021, 28 september). identity provider. SearchSecurity. Geraadpleegd op 1 juni 2022, van https://www.techtarget.com/searchsecurity/definition/identity-provider

### What are the advantages of using an identity provider for security?

It is easy to implement and can be used for a variety of applications. Also as owner of the application you don&#39;t need to save user identity information, the users identity is seperate from the application. Also because of not saving user data you don&#39;t need to take security measures against bad actors at least not for the login.

Identity providers (IdP&#39;s): wat zijn dat en waarom heeft u ze nodig | Okta. (2022, 1 juni). Okta, Inc. Geraadpleegd op 1 juni 2022, van https://www.okta.com/nl/identity-101/why-your-company-needs-an-identity-provider/

### What are some of the most popular providers?

Some examples are github, google, facebook and microsoft are some of the most popular providers which most people probably will have an account on at least one of these services

Lutkevich, B. (2021, 28 september). identity provider. SearchSecurity. Geraadpleegd op 1 juni 2022, van https://www.techtarget.com/searchsecurity/definition/identity-provider

### What is oAuth2?

Is a standard designed to allow a website or application to access resources hosted by other web apps on behalf of a user. oauth2 provides consent and restricts access on behalf of the user without ever sharing user credentials. There are different roles within oauth2: resource owner, client, resource server and authorization server.

### How does oAuth2 work

the Client must acquire its own credentials, a client id and client secret, from the Authorization Server in order to identify and authenticate itself when requesting an Access Token.

the steps in order to receive a token:

1.The Client requests authorization (authorization request) from the Authorization server, supplying the client id and secret to as identification; it also provides the scopes and an endpoint URI (redirect URI) to send the Access Token or the Authorization Code to.

2.The Authorization server authenticates the Client and verifies that the requested scopes are permitted.

3.The Resource owner interacts with the Authorization server to grant access.

4.The Authorization server redirects back to the Client with either an Authorization Code or Access Token, depending on the grant type, as it will be explained in the next section. A Refresh Token may also be returned.

5.With the Access Token, the Client requests access to the resource from the Resource server.

What is OAuth 2.0 and what does it do for you? - Auth0. (2022, 1 juni). Auth0. Geraadpleegd op 1 juni 2022, van https://auth0.com/intro-to-iam/what-is-oauth-2/

### What is a jwt token?

JSON web token is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a json object. This information can be trusted and verified because it is digitally signed. Jwts can be signed using a secret or a public/private key.

###

### When should i use a web token?

Jwts are useful for authorization and information, authorization is the most common way for using a jwt. once the user is logged in every subsequent request will include a jwt allowing the user access to resources , services etc. Single sign on is a widely used feature that uses jwt.

For information exchange jwts are a good way of safely transmitting information between parties. Because jwts can be signed you can be sure the senders are who they say they are, you can also verify that the content inside of the header hasn&#39;t been tampered with.

### What is a json web token structure?

In its compact form JSON web tokens consist of three parts which are: Header, payload and signature.

The header typically consists of two parts: the type of token and the signing algorithm used such as HMAC SHA256 or RSA.

example:

![](RackMultipart20220601-1-redtt6_html_5f047b7ea9573f20.png)

The second part of the jwt is the payload which contains the claims, claims are a statement about an entity and additional data. There are three types of claims: registered, public and private claims.

-Registered claims there are a set of predefined claims which are not mandatory but recommended to provide a set of useful interoperable claims, Some of them are: iss (issuer), exp (expiration time), sub (subject), aud (audience).

-Public claims These can be defined at will by those using JWTs. But to avoid collisions they should be defined in the IANA JSON Web Token Registry or be defined as a URI that contains a collision resistant namespace.

-Private claims These are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.

example of the payload:

![](RackMultipart20220601-1-redtt6_html_63b58ca6056bd970.png)

And last is the signature to create this part you have to take the encoded header, the encoded payload, a secret and the algorithm specified in the header and sign it. The signature is used to verify the token wasn&#39;t changed along the way and in case of tokens signed with a private key, it can also verify that the sender of the jwt is who it says it is.

### How do JSON web tokens work?

In authentication when a user logs in successfully using their credentials a json web token will be returned.

auth0.com. (2022, 1 juni). JWT.IO - JSON Web Tokens Introduction. JSON Web Tokens - Jwt.Io. Geraadpleegd op 1 juni 2022, van https://jwt.io/introduction

#

###

###

###

###

###

# Conclusion

In conclusion there are many identity providers around, they carry a lot of advantages opposed to not using one. oauth2 is the standard for external authentication and authorization. oauth 2 works in 5 steps:

1.The Client requests authorization (authorization request) from the Authorization server, supplying the client id and secret to as identification; it also provides the scopes and an endpoint URI (redirect URI) to send the Access Token or the Authorization Code to.

2.The Authorization server authenticates the Client and verifies that the requested scopes are permitted.

3.The Resource owner interacts with the Authorization server to grant access.

4.The Authorization server redirects back to the Client with either an Authorization Code or Access Token, depending on the grant type, as it will be explained in the next section. A Refresh Token may also be returned.

5.With the Access Token, the Client requests access to the resource from the Resource server.

# Sources

[https://oauth.net/2/](https://oauth.net/2/)

[https://auth0.com/blog/5-massive-benefits-of-identity-as-a-service-for-developers/](https://auth0.com/blog/5-massive-benefits-of-identity-as-a-service-for-developers/)

[https://auth0.com/intro-to-iam/what-is-oauth-2/](https://auth0.com/intro-to-iam/what-is-oauth-2/)

[https://jwt.io/introduction](https://jwt.io/introduction)
