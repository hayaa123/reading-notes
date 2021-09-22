# [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

## What is OAuth?

open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential

## Give an example of what using OAuth would look like.

when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.

## How does OAuth work? What are the steps that it takes to authenticate the user?

1- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

2- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

3- The first site gives this token and secret to the initiating user’s client software.

4- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

5- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

6- The user approves (or their software silently approves) a particular transaction type at the first website.

7- The user is given an approved access token (notice it’s no longer a request token).

8- The user gives the approved access token to the first website.

9- The first website gives the access token to the second website as proof of authentication on behalf of the user.

10- The second website lets the first website access their site on behalf of the user.

11- The user sees a successfully completed transaction occurring.

## What is OpenID?

OpenID is for humans logging into machine

# [Authorization and Authentication flows](https://auth0.com/docs/authorization/flows)

## What is the difference between authorization and authentication?

Authentication confirms that users are who they say they are. Authorization gives those users permission to access a resource. [okta](https://www.okta.com/identity-101/authentication-vs-authorization/#:~:text=What's%20the%20difference%20between%20authentication,permission%20to%20access%20a%20resource.)

## What is Authorization Code Flow?

used to obtain an access token to authorize API requests. [mendele](https://dev.mendeley.com/reference/topics/authorization_auth_code.html#:~:text=Authorization%20code%20flow%20is%20used,token%20to%20authorize%20API%20requests.&text=Access%20tokens%2C%20obtained%20using%20authorization,requests%20for%20all%20API%20resources.)

## What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

an OpenId Connect flow specifically designed to authenticate native or mobile application users  [onelogin](https://developers.onelogin.com/openid-connect/guides/auth-flow-pkce#:~:text=The%20Authorization%20Code%20Flow%20%2B%20PKCE,Proof%20Key%20for%20Code%20Exchange.)


thaks for reading :D 