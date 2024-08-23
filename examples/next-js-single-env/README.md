
# Sitecore XM Cloud External App - Single Environment Example

This example demonstrates how you can create a separate web application that interacts with the Sitecore XM Cloud environment, using a single Authoring Graphql Client credentials.

Unlike the multiple environments example, the security is around the user adding the client information for their environment. This is simpler because the connection information is stored in Environment Variables for the app. However this creates a new challenge, because users to the app, need to be authenticated. To get around this, users to the app, will be forced to login to the XM Cloud application in order to authenticate and start using the app. Obviously other identity providers could be used instead here.

Looks like two options here.

1. Use Sitecore Auth
    - This is less secure, because someone just needs to be able to login to cloud portal, not necessarily have access to XM Cloud etc.
2. Use External Provider like AAD or Okta etc.

Looks like XM Cloud + Cloud Portal uses oAuth2 with Authorization Code Flow grant type.  So this might be an initial screen that takes user to auth.sitecorecloud.io authenticates and sends you back with an access token.