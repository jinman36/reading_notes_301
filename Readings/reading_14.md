# Reading Assignment - 14

## Readings: Authentication

### Date 11-2-2021

1. [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

What is OAuth?
Open standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to thier assets.

Give an example of what using OAuth would look like.
Signing into one website and being allowed signed in previlages in linked websites

How does OAuth work? What are the steps that it takes to authenticate the user?
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.
12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

What is OpenID?
It is another security technology - openID is focused on authorization as opposed to authentication like OAuth is.

1. [Authorization and Authentication flows](https://auth0.com/docs/authorization/flows)

What is the difference between authorization and authentication?
What is Authorization Code Flow?
What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
What is Implicit Flow with Form Post?
What is Client Credentials Flow?
What is Device Authorization Flow?
What is Resource Owner Password Flow?

## Things I want to know more about
