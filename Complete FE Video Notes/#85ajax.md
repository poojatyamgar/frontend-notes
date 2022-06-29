---
marp: true
---


#       JSON

+ JS Object Notation is a simple text format.
+ Looks like a JS object
+ Can be converted into one easily for JS processing
  of server data
+ No complicated parsing and translations.
+ Compact as a string, open as a JS object.
+ Lightweight, language and platform independent.
+ Important for backend programming, NoSQL databases
  like MongoDB.

---

#       An example page with washington

#       Advantages Of JSON

+ Its syntax is very easy to use
+ Its syntax is very small and light-weighted that's the reason
  that it executes and responds in a faster way.
+ JSON has a wide range for the browser support compatibility
  with the operating systems.
+ It doesn't require much effort to make it all browser compatible.
+ On the server-side parsing is very fast with JSON
+ If parsing is fast on the server side then the user can get the 
  fast response.

---

#       Disadvantages of JSON

+ There is no error handling in JSON, if there be a slight mistake
  in the JSON script then you will not get the structured data
+ So need to verify JSON before use always

---

#        Data Types

+ In JSON, values must be one of the following data type:
   + a string
   + a number
   + an object(JSON object)
   + an array
   + a boolean
   + null

+ JSON values cannot be one of the following data types:
  + a function
  + a date
  + undefined

---

#        Sending JSON

+ Convert for JS object tpo JSON string.
+ JSON.stringify() accomodates everything except functions
+ Send it as data over a function call or async call.
+ Can use JSON string with other string to get the desired data.
+ jQuery.getJSON(url [, data] [, success])
+ Load JSON-encoded data from the server using a GET HTTP request.

---

#         Receiving JSON

+ Obtain JSON string then convert to JS object
+ JSON.parse(JSONdata);
+ Use this as data to iterate over and display in HTML
  page e.g. as a table.
+ Can use JSON string with other string to get the desired
   data to display.