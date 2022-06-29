---
marp: true
---

#       Module 11

+ Serving and retrieving data
  to a website
+ Synchronous Vs Asynchronous loading
+ Set up and handle AJAX requests and 
  responses
+ JSON
+ XML
+ Processing JSON data
+ JSON Vs XML

---

#    Requests And Responses

+ The Hypertext Transfer Protocol (HTTP) is designed to
  enable communications between clients and servers.
+ HTTPS works as a request-response protocol between
  a client and server.

+ Browser → REQUEST → Server
  Browser ← RESPONSE ← Server

#      Synchronous Vs Asynchronous

+ Two types of requests - synchronous and asynchronous
+ synchronous - one instruction at a time
+ asynchronous - execution is done in a separate thread
                 or process
+ JS is synchronous language.
+ A browser is made up of- JS engine, Event Queue, HTML 
  rendering, webGL, HTTP Requestor.
+ JS engine is synchronous, but HTTP requestor is 
  asynchronous.

---

#       Advantages of Asynchronous

+ Speed is enhanced as there is no need to reload the page again
+ Making asynchronous calls to a web server - client browsers avoid
  waiting for all the data to arrive before starting of rendering.
+ Form validation can be done in real-time with it.

+ Browser → REQUEST → Server
  Browser ← RESPONSE ← Server

  The time taken between request and response is known as "request time"
+ Multitasking
+ To make full utilization of the CPU and other resources use 
  asynchronous calls.

---

#         Timeouts and intervals

+ Tradiotional methods JS has available for running code
  asynchronously
+ After a set time period has elapsed, or at a regular interval
  do the task.
+ Cooperative asynchronous JS
+ setTimeout(), setInterval()

---

#        Get and Post

+ The two methods to request data from server - Get and Post
+ GET/index.html?name=SkillLync http/1.1
+ Method, URI string, Query string, http version
+ HTTP response status
   + 200, OK
   + 404, Not Found
   + 403, Forbidden
   + 500, Internal Server Error

---

#      GET

+ The GET method may return cached data.
+ GET requests should never be used when
  dealing with sensitive data as it passes
  it in the query string
+ GET requests have length restrictions

---

#     POST

+ The POST method never caches data.
+ POST requests sends data without
  any length restrictions
+ POST is used for working with 
  sensitive data

---

#    AJAX

+ Asynchronous Javascript And XML
+ Reads data from a web server - after the page has loaded
+ Updates a web page without reloading the page
+ Sends data to a web server in the background
+ AJAX uses a combination  of :
   + A browser built-in XMLHttpRequest object (to request data
     from a web server)
   + Javascript and HTML DOM (to display or use the data) 

+ Browse → HTTP Request (method: GET
                         path: /index.html) → Server

  Browser ← HTTP Response (status: 200
                           content-type: text/html;
                                         charset=UTF-8) ← Server

---

#       XMLHttpRequest object

+ All modern browsers support the XMLHttpRequest object can be
  used to exchange data with a web server behind the scenes
+ The XMLHttpRequest object can be used to exchange data with
  a web server behind the scenes.
+ The object has properties and methods.

---

#      XMLHttpRequest Object Methods

+ new XMLHttpRequest() - creates a new XMLHttpRequest object
+ abort() - cancels the current request
+ getAllResponseHeaders() - returns header information
+ getResponseHeader() - returns specific header information
+ open(method, url, async, user, psw) - Specifies the request
   + method: the request type GET or POST
   + url: the file location
   + async: true(asynchronous) or false(synchronous)
   + user: optional user name
   + psw: optional passwords

---

#      XMLHttpRequest Object Properties

+ Onreadystatechange - Defines a function to be called when the readyState
                       property changes
+ readyState - Holds the status of the XMLHttpRequest
    + 0 : request not initialized
    + 1 : server connection established
    + 2 : request received
    + 3 : processing request
    + 4 : request finished and response is ready
+ responseText - Returns the response data as a string
+ Status - Returns the status-number of a request

---

#         The AJAX process

+ JS code and HTTP Requestor work together independently
+ The HTTP requestor is given address of the JS function 
  response handler - callback function
+ If in AJAX, we use the code differently, then requests
  and responses can get mixed and a race condition might 
  get developed.
+ Hence mind the sequence!
