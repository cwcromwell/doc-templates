# Reference Section

## About the Reference Section 

The reference section is the main event for your API documentation. New users will start with other documents to help them get going, but experienced users will refer more frequently to the reference section for the detailed information they need to make use of the API. 
The reference section should contain a full listing of endpoints, methods, and parameters

## The General Contents 

The reference section is generally a collection of short entries, arranged in alphabetical order. 

### Parts of the Reference Entry

Each reference listing should contain:
* The HTTP method, if applicable (GET, POST, PATCH, DELETE)
* An example of the syntax
* A description of the endpoint in question (What is it for, and what can it do?)
* All the parameters for each endpoint (At a minimum: name, data type, description, comments. See below for more information)
* An example request
* An example response
* Response schema

### More about the Parameters 

Each detailed reference entry should contain all the information a user might need to know when using a parameter (attributer), whether that parameter is part of the request or the response.
If a parameter is accepted by the endpoint, it should be listed -- the api will be difficult to understand if usable parameters are missing.

Include these: 

   * Description of what the parameter does 
   * When and why would the user need to use the attribute
   * The data type
   * All the acceptable values, if there is a limited set of options
   * Whether the parameter is required or optional (This goes for response attributes as well. Are they always returned, or only sometimes?)

### Special Reference Topics

These have to be covered someplace in your documentation. They are sometimes included in the reference chapter, but don't have to be. 

* Authentication.
* Error-handling. Make sure users can find an explanation for any error code they might receive. 
* Throttling. (Limiting the number of requests a user can make within a period of time.)

## Best Practices

If more than one endpoint or parameter can get the job done, explain which one pertains to which situation. (Each probably exists for a specific reason, but the user needs to know.)

Each reference entry should include both a syntax and a working example. 

Example code should be followed by extensive comments that explain how it works. Some users get started by playing with the example code and they'll get frustrated if they cannot make it work. For them, the example should be followed by brief instructions about which parts of the code they need to replace with their own authentication keys and user ids. They need warnings about common errors that will prevent the request from working. 

Structure the information in a consistent way for all endpoints. Include every parameter, but also list them the same way, for example in alphabetical order or in the order they are used in the request or response. 

## Examples

examples:
https://developers.google.com/gmail/api/v1/reference



