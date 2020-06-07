# pluralsight_http_learn
pluralsight course on HTTP fundamentals </br>

# Course Note:

## URL

http://www.food.com/recipe/grilled-cauliflower </br>
http://www.food.com => URL = Uniform Resource Locator </br>
https:// => URL schema </br>
www.food.com => host (DNS server will resolve it and found the ip address) </br>
/recipe/grilled-cauliflower => URL path </br>
/recipe/grilled-cauliflower looks like a FS system path, sometimes a web server did map FS to url path. But nowadays most of web server has a web service running to handle URL path (router) </br>

Note: Sometimes single web may need make multiple HTTP requests </br>

## HTTP and IIS
IIS is a web server application which can map physical path to url (basically check if resource is available in local FS to respond the HTTP request) </br>

## Ports, Queries, Fragments
http://www.food.com:80/recipes/squash </br>
80 is default HTTP request port. web server will defaultly listen to 80 port  </br>

http://bing.com/search?q=jabotica </br>
search => path </br>
q=jabotica => query string (No standard, depends on how web application business logic to handle the query)  </br>

http://wiki.org/wiki/javabb#Description </br>
Description => fragment  </br>
This is to help navigate a part of resource that the client requests (web server doesn't respect it, it is all about web browser showing the current fragment of response/resource)  </br>

http://host:8080/path?q=query#fragment this is the general format </br>

## URL Encoding
pay attention to Unsafe characters like space </br>
Safe Character: A-Z a-z 0-9 - . _ ~ ( ) ' ! * : @ , ; </br>
Unsafe Character: % < > [ ] { } | \ ^ </br>
If you still want to use unsafe character, you have to escape them for example 'space' is %20 </br>

## Content Type
When host responses, it will response content and content type, so that web browser can render correct content type </br>
MIME type: Multipurpose Internet Mail Extensions (came from email originally) </br>
MIME type example: image/png  application/json  text/plain  text/html text/plain </br>

## Content Negotiation
When client request resource, single URL may have different representation in the host(web server). client can specify which type will be accepted on client side </br>
For example, French version of www.google.com, you can change internet option in browser so request will be sent along with content negotiation </br>

## HTTP Messages
HTTP standard define the protocol so that client and server can understand each other </br>

## HTTP Methods:
GET,POST - In most HTML web application </br> 
(PUT,DELETE,HEAD)- mostly never used in web application </br>
Note: POST method comes with form data </br>


