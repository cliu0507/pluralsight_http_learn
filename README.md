# pluralsight_http_learn
pluralsight course on HTTP fundamentals </br>

# Course Note:

# URL

http://www.food.com/recipe/grilled-cauliflower </br>
http://www.food.com => URL = Uniform Resource Locator </br>
https:// => URL schema </br>
www.food.com => host (DNS server will resolve it and found the ip address) </br>
/recipe/grilled-cauliflower => URL path </br>
/recipe/grilled-cauliflower looks like a FS system path, sometimes a web server did map FS to url path. But nowadays most of web server has a web service running to handle URL path (router) </br>

Note: Sometimes single web may need make multiple HTTP requests </br>

# HTTP and IIS
IIS is a web server application which can map physical path to url (basically check if resource is available in local FS to respond the HTTP request) </br>

# Ports, Queries, Fragments
http://www.food.com:80/recipes/squash </br>
80 is default HTTP request port. web server will defaultly listen to 80 port  </br>

http://bing.com/search?q=jabotica </br>
search => path </br>
q=jabotica => query string (No standard, depends on how web application business logic to handle the query)  </br>

http://wiki.org/wiki/javabb#Description
Description => fragment  </br>
This is to help navigate a part of resource that the client requests (web server doesn't respect it, it is all about web browser showing the current fragment of response/resource)  </br>

http://host:8080/path?q=query#fragment this is the general format </br>
