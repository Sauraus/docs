::: warning
Since the Resource Owner Password Grant (ROPG) flow involves the client handling the user's password, it **must not be used by third-party clients**. In this flow, the user's username and password are exchanged directly for an Access Token.

Only consider using it when there is a high degree of trust between the user and the application and when other authorization flows (such as redirect-based flows) are not available.

Instead, Auth0 recommends: 
* For confidential clients, like Regular Web Applications, use the [Authorization Code Flow](/flows/concepts/auth-code).
* For public clients, like Native/Mobile Apps and Single-Page Applications, use the [Authorization Code Flow with PKCE](/flows/concepts/auth-code-pkce).
:::
