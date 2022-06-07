---
marp: true
---

#    Request

+ xhttp.onreadystatechange = function() { // "onreadystatechange" → Event triggered at 
                                          // change in readyState
    if (this.readystate == 4 && this.status == 200 ){
        document.getElementById("test").innerHTML = this.responseText;

    }
   };
  xhttp.open("GET", "ajax_info.txt", true);
  xhttp.send()
  or xhttp.send("jsonstring");

+ If want asynchronous, add false as async argument

---

#    Response

+ Adding different callback function for different AJAX responses
  so responses are handled separately
+ Response property - reqobj.responseText
+ Response methods - getAllResponseHeaders()
+ this.getAllResponseHeaders() in onreadystatechange function


#    jQuery and AJAX

+ $(selector).load(URL, data, callback);
+ The callback function can have different parameters:
      + responseTxt - contains the resulting content if the call succeeds
      + statusTxt - contains the status of the call
      + req - contains the XMLHttpRequest object
+ $.get(URL, callback);
+ $.get(url[, data][, success][, dataType])
+ $.post(URL,data,callback);
+ $.post(url[, data][, success][, dataType])

#    jQuery and AJAX

+ jQuery.getScript(url, [success])
+ Load a JS file from the server using a GET HTTP request, 
  then execute it.

#    Promises

+ promise ?
+ Promise represents the eventual result of some sort of
  operation typically an async operation.
+ States
   + Pending
   + fulfilled(resolved)
   + rejected

#     Async await

+ More recent additions to the JS language
+ 'async' functions and the 'await' keyword
+ Part of ECMAScript 2017 JS edition
+ Async await exactly same as promises just
  a simpler syntax.
+ Makes asynchronous code easier to write 
  and to read afterwards.

#    The Fetch API

+ Fetch API ?
+ Using fetch API to get JSON response from server