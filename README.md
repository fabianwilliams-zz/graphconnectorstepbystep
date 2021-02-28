# graphconnectorstepbystep
Creating a Microsoft Search Graph Connector via the API step by step with an External Files scenario

**WHAT**: This is a Gist for an end to end scenario demo and blog to create and consume a Microsoft Search Graph Connector
**WHO**: the user persona in the Index Json above represents a user in your active directory that you want to have access to this data
**WHEN**: you will be setting this up after you have created your App Registration in Azure AD. See order of operations below
**WHERE**: you will be doing this anywhere you can fire off an API, for simplicity sake you can do this in Postman but you can do this from your own published Web API service
**WHY**: because you are here to learn
**HOW**: see my blog post for details

**Order of Operations**

1. createexternalconnection.json as a POST to https://graph.microsoft.com/beta/external/connections
2. createexternaldataschema.json as a POST to https://graph.microsoft.com/beta/external/connections/fabsdemofilesdrivealpha/schema
3. createindexforschema.json as a PUT to https://graph.microsoft.com/beta/external/connections/fabsdemofilesdrivealpha/items/{{uniqid}}
4. createadaptivecardforresulttype is used in the Search Admin Center after your create your Search Vertical

