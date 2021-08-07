# Authentication

## OAuth

***

1. **What is OAuth?**
   *  Open Authorization, s an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

2. **Give an example of what using OAuth would look like.**
   * When you go to log onto a website and it offers one or more opportunities to log on using another website's/service's logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

3. **How does OAuth work? What are the steps that it takes to authenticate the user?**
   1. The first website connects to the second website on behalf of the user, using OAuth, providing the user's verified identity.
   2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
   3. The first site gives this token and secret to the initiating user's client software.
   4. The client's software presents the request token and secret to their authorization provider (which may or may not be the second site).
   5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
   6. The user approves (or their software silently approves) a particular transaction type at the first website.
   7. The user is given an approved access token (notice it's no longer a request token).
   8. The user gives the approved access token to the first website.
   9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
   10. The second website lets the first website access their site on behalf of the user.
   11. The user sees a successfully completed transaction occurring.
   12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work acrossthe web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. **What is OpenID?**
   * OpenID enables an end-user to communicate with a relying party. This communication is done through the exchange of an identifier or OpenID, which is the URL or XRI chosen by the end-user to name the end-user's identity. An identity provider provides the OpenID ***authentication.***

[Authorization and Authentication Flows](https://auth0.com/docs/flows)