

# Sitecore XM Cloud External App - Multiple Environments Example

This example demonstrates how you can create a separate web application that interacts with the Sitecore XM Cloud environment, using multiple Authoring Graphql Client credentials.  This scenario is a little more complex, because a user will add different environments for their session. Ideally these configurations should last for a certain amount of time. An additional data store may be used here, which obviously adds complexity to the solution.

Each user does not need to be authenticated to use the app however, but instead they can come, add in their environment credentials and then interact with their Sitecore Cloud environment (This will start with XM Cloud, but could be extended to handle Personalize, CDP, Content Hub One and other tools).