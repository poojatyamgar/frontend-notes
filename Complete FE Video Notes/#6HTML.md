---
marp: true
---

#  Understanding the Head

+ <html lang="zxx">
+ <meta charset="UTF-8">otherwise Mojibake
+ <meta name="description" content="Skill-Lync Master's course">
+ <meta name="viewport" content="width=device-width, initial-scale=1.0">
+ Supporting files
   <link rel="icon" type="image/png" href="images/flavicon.png">

---

# DOM structure 

+          <html>
       ↓            ↓
     <head>       <body>  
       ↓            ↓
     <title>      <h1> <p> 
     <meta>             ↑→ Attribute "id"

---

# Anatomy of HTML syntax

+ Tags, Attribute

                    Element
                       ↑
       ----------------------------------------------------               
         ↓                            ↓                  ↓
    Start tag<p>                    Content              End Tag</p>
        ↓                            This is 
    Attribute1 Id="firstp"           my first paragraph
    Attribute2 Class="para"

---

