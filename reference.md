# The API Reference Documentation

## About the Reference Section

The reference section is the foundation of your API documentation. It consists of a full listing of endpoints (or operations, if you prefer to call them that).

You might offer step-by-step instructions for getting started and for completing specific tasks; nevertheless, all your users will need to refer to the reference documentation to make use of the API.

## The contents and general structure

Like any reference document, the API reference section is generally a collection of short entries, arranged in some kind of order. For example, the listings might be alphabetical or might be sorted by function -- there's more than one way to do it.  

### Parts of the Reference Entry

Each reference listing should contain:

* The HTTP method. The most common are GET, POST, PATCH, and DELETE.
* An example of the URL syntax. This is important if any of the parameters are included in the URL. For example: `../members/{member_id}`, where the bracketed item at the end is a placeholder for the specific id number for the member whose information we need to see.
* A description of the endpoint in question (What is it for, and what can it do?)
* Complete details for _every_ parameter that can be included in a request. And that goes for the parameters of _every_ endpoint. At a minimum, your readers need to know: name, data type, description, and whether or not the parameter is required or optional. (See below for more about this subject.)
* An example request. Ideally, one that users can cut-and-paste into the terminal or a script.
* An example response. Users of your API need to know what the response is supposed to look like
* An explanation of response properties. Just like the request, users need to know the name, data type, and description of any property that can be included in the response object.

### More about describing the parameters

Each reference entry should contain all the information a user might need to know when using the individual parameter, request body attribute, or response body property.
The first rule of reference documentation is to include all of them. If a parameter is accepted by the endpoint, it should be listed -- because the api will be difficult to understand if usable parameters are missing or if it returns properties in the response object without explaining what they are for.

Each entry should include these:

   * Description of what the parameter does
   * When and why would the user need to use the parameter, request attribute, or response property.
   * The data type.
   * All the acceptable values, if there is a limited set of options (for example, a value might be limited to True/False; or you might have a unique parameter that requires users to choose between `[hi | medium | low]` or `[ DES | AES | RSA ]`. Remember to enumerate the options and explain what each of them means.
   * Whether every parameter is required or optional. It can be frustrating to try to make the API call when you're not sure which attributes are essential for the request to be processed. (This goes for response attributes as well. Are they always returned, or only sometimes? Users need to know this if they're handling the response programmatically.)
   * On a similar note, make sure users know when an attribute is not to be included. Suppose that providing an account id when creating a new account would cause the request to error out. Let users know that they don't need the attribute by showing an example request that doesn't include the id. It's helpful to show only the attributes that are necessary for the request and that are likely to be used, especially if the request object is large.


### Special Reference Topics

These have to be covered someplace in your documentation. They are sometimes included in the reference chapter, but don't have to be.

* Authentication.
* Error-handling. Make sure users can find an explanation for any error code they might receive.
* Throttling. (Limiting the number of requests a user can make within a period of time.)


## Best Practices

These tips make your documentation easier to read and use:

* If more than one endpoint or parameter can get the job done, explain which one pertains to which situation. (Each probably exists for a specific reason, but the user needs to know.)
* Each reference entry should include both a URL syntax and a working example.
* Structure the information in a consistent way within each entry. For example in alphabetical order or in the order they are used in the request or response--but use the same organizing principle in every entry.

## Examples

examples:
https://developers.google.com/gmail/api/v1/reference
