---
marp: true
---

#       Storing JSON

+ Just like storing a text but in a better format 
  to use it easily next time
+ The file type for JSON file is ".json"
+ The MIME type for JSON text is "application/json"

---

#         Serialisation

+ Serialise - encode to JSON from server side script
+ De Serialise - parse from JSON at client side script
+ What is serialize() in jQuery ?
   In the standard URL-encoded notation jQuery serialize()
   is used to create the text strings.
   $("button").click(function(){
       $("div").text($("form").serialize());
   });

---

#        Traversing JSON

+ Most programming languages have great libraries to parse
  and generate JSON data e.g. JSONB in Java.
+ The same way JavaScript objects can be used as JSON, 
   JavaScript array can also be used as JSON.
+ 2 ways to parse JSON - 
    + Object parsing syntax
    + Associate arrays syntax
+ Parsing a non JSON object eg data, function

---

#          The for in loop

+ Loop though JSON keys and values
+ Loop through JSON arrays
+ Nested JSON objects and arrays

---

#        Other JSON manipulations

+ Adding JSON attributes
+ Deleting JSON attributes
+ Check if a key exists in JSON

---

#        Same-origin security feature

+ Browsers use same source, same origin rule. They do not allow access
  across domains
+ Other sources are not allowed to be accessed by the website
+ We need CORS to tell browser what sources are safe.
+ Cross-origin resource sharing (CORS) - mechanism that allows
  resources on a web page to be requested from an outside domain
+ This domain is other than the one from which the first resource
  was served.
+ A web page may then freely embed cross-origin images, stylesheets,
  scripts, iframes, and videos.

---

#           XML

+ eXtensible Markup Language
+ XML Does Not Use Predefined Tags
+ Element-attribute-content
     <mydefinition>
           This is the structure I define. Mah life, mah rulez!
        <firstpart>
            <description>This is the first part</description>
        </firstpart>
        <secondpart>
            <description>This is the second part</description>
        </secondpart>
        <thirdpart>
            <banana>This is the third part</banana>
        </thirpart>
    </mydefinition>

---

#                XML

+ XML - structure data  Vs HTML - display data
+ New rules or tags can be added in your xml later
+ Great to share understandable data - 
   + <thisismostimp>First wish</thisis mostimp>
   + <thisisprioritytwo>Second wish</thisisprioritytwo>
   + So on...
+ Stores and shares as text so we don't lose data due to
  conversions in different formats

---

#               Rules for XML

+ Should have root tag always
+ Should have closing tag always
+ Proper nesting is important to validate XML
+ Attributes in quotes
   + <mywish priority="first"></mywish>
+ Comments
   + <!--This is a comment-->

---

#          Rules for XML

+ Element names
   + are case-sensitive
   + must start with a letter or underscore
   + cannot start with the letters xml (or XML, or Xml, etc)
   + can contain letters, digits, hyphens, underscores, and periods
   + cannot contain spaces

---

#           Traversing XML

+ XML is a tree structure
+ Nodes
   + Parent
   + Children
   + Siblings
   + element node
   + attribute node
   + text node
+ Properties - nodeName, nodeType
+ All major browsers have a built-in XML parser
  to access and manipulate XML

---