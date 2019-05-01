# SpringBoot-ContentNegotiationManager

    Usual scenarios we specify if a method should return a response either as xml,json,html or some other type. But it may happen that we need the same method to return a response of different type depending on the incoming request. 
For example we have a Server application which return the list of employees. We are having 2 UI applications using the same server method to get the list of employees. But one requires xml and the other json. 
This is where content negotiation comes into picture. As name suggests it negotiates the response type based on the request. This content negotiation can be achieved in following ways-

# Using Path Extension -
  In the request we specify the required response type using the extension like .json,.xml or .txt. This has the highest preference
# Using url parameter - 
  In the request we specify the required response type using the url parameter like format=xml or format=json. This has the second highest preference
# Using Accept Headers - 
  When making a request using HTTP we specify required response by setting the Accept header property. Its something like this
