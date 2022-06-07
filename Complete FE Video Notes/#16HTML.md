---
marp: true
---

#  Adding Youtube Videos

+ Upload the video on YouTube. Check the youtube embed script.
  <iframe src=“videoURL”> 
+ Use the width and height attributes to specify the dimension of the player
+ Add other parameters to the URL as required- 
  <iframe width="560" height="315" 
  src="https://www.youtube.com/embed/L4GPkB2n9Gg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
  </iframe> 

---

# Geolocation

+ For rendering maps, giving certain services based on location.
+ getCurrentPosition() method is used in the script to gain this information.
+ What about users’ privacy?

---

# Web Storage

+ With web storage, web applications on loading, can store data within the user's browser locally.
+ Better than cookies.
+ window.localStorage- stores data without expiry
+ window.sessionStorage- stores data only for one session
+ Interview question- What are the different types of Web Storage provided by HTML5? Explain 
  the key differences between localStorage and sessionStorage objects.

# Web Workers

+ Ever experienced a page becoming unresponsive due to a script never finishing?
+ A web worker is a JavaScript that runs in the background, independently of other scripts, 
  without affecting the performance of the page. 
+ You can continue to use the application, while the web worker runs in the background.

---

# Drag and Drop

+ In HTML, any element can be dragged and dropped.
<img draggable="true">

---

# SS Event

+ Server-Sent Events (SSE) allow a web page to get updates from a server.
+ What’s new in this?
+ Examples: Facebook/Twitter updates, stock price updates, news feeds, sport results, etc.

---

# Application Cache

+ What’s a cache?
+ Application Cache- Introduced in HTML5. 
+ Application is accessible without an internet connection after loading once.
   + Offline browsing
   + Speed
   + Reduced server load
+ A Manifest file is a simple text file, that tells the browser what to cache and what not to cache.

---

# XHTML - Best Practice

+ XHTML stands for EXtensible HyperText Markup Language. Rules for this is maintained by the W3C.
+ <!DOCTYPE> is mandatory
+ <html>, <head>, <title>, and <body> are mandatory
+ Elements must always be properly nested, closed, in lowercase, be quoted
+ Attributes should be in lowercase and minimization is forbidden
+ Use W3C validator for HTML5 errors

---

# Summary

+ Document structure
+ Different Tags
+ Forms and inputs
+ Colors, classes and ids
+ Graphics
+ Media
+ HTML APIs
+ Best practices

---