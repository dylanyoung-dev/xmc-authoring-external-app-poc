
# Sitecore XM Cloud External App - Single Environment Example

This example demonstrates how you can create a separate web application that interacts with the Sitecore XM Cloud environment, using a single Authoring Graphql Client credentials.

Unlike the multiple environments example, the security is around the user adding the client information for their environment. This is simpler because the connection information is stored in Environment Variables for the app. However this creates a new challenge, because users to the app, need to be authenticated. To get around this, users to the app, will be forced to login to the XM Cloud application in order to authenticate and start using the app. Obviously other identity providers could be used instead here.