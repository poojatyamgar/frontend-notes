---
marp: true
---

# CSS rule conflict resolution

      + An element can have (Inline style, Internal style, External style).
      + The conflict is which style would the HTML choose if it has style present in all 3.
         To overcome this, we have the Style Hierarchy

---

# Style Hierarchy

      + Used to create flexibility and changes from global styles.
            + Overriding (Internal overrides external, inline overrides internal)
            + Merge (2 definitions on the same element have different property, then all those 
              property  are implemented on it.) 
            + Inheritance (The properties we define under an element is implemented on all of 
              its children as well, [unless it is overridden].)
            + Specificity 

---

            + Specificity
                 +  The higher the number, the more specific is the selction.

                    id=100
                    class=10
                    pseudo/elements=1
                    inline=1000
                    
                    The styling specificity is measured according to the addition, of the particular style.

---

                        div span{
                    
                          }; // The specificity would be (1+1=2)

          // In CSS, we can mention ids in div tags, like 

                       div[id=a]{ // (1 = 1) "Less Specific"

                        }; 

                    // OR

                        #a{  // (100) "More Specific"

                         };

---

          Note:
                #foo {} has a specificity of 1-0-0 while [id="foo"] {} selects the same element but has a much lower specificity of 1-0. 

                Correct - that's because CSS itself does not have any mappings from ID/class selectors to any particular attribute,  
                          so any attribute selector will have the same specificity regardless of attribute name.
                          This mapping is performed by the browser according to document semantics, not CSS semantics.
                          It just so happens that attribute and class selectors share the same specificity (most likely to keep things simple).

---

               +    ID selectors have a higher specificity than attribute selectors.
               +    Use of !Important 

                      div:first-child{
                            background-color: red !important
                            height: 100px;
                            width: 30px;
                           }
                      // It doesn't matter what specificity number it has, the element which has "!important" in it
                         makes it win(even more than inline styling). It will not be overridden.