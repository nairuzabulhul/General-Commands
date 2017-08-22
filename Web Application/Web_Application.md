### Web Application :

- HTTP Analysis
- HTTPS Analysis 
- BurpSuite


#### HTTP Analysis:

- __netcat__
    
        EX: nc www.google 80 

- When connecting with netcat:

        EX:
            GET / HTTP/1.1
            HOST: www.google.com




### HTTPS Analysis:

- __OpenSSL__
    
        EX:


### BurpSuite Tools:

- __Proxy:___
        - intercepts every request 
        - Multiple actions can be performed on requests
        - Setting a scope is very important to weed out irrelevant requests
        - Filter the  scope to show only relevant URLs
        - Add the scope to the proxy "Intercept" by checking the URL box 
        - Any other URLs that are not included in the scope would be ignored by the
          proxy intercept
        - HTTP logins are shown in BurpSuite and can be modified via proxy 
        
    __Target__
        - Bold objects are objects that are reguested by BurpSuite user
        - Grey objects are pobjects that are automatically pull out by the program
    
    __Spider__:
         - Crawls web pages within the speciifc scope
         - For forums it is better to choose the option prompot for guidance to avoid uncessary form submissions
    
    __Repeater__: 
            - Checks how the application behaves 
