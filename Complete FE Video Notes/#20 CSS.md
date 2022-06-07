---
marp: true
---

# Pseudo classes and pseudo elements

   + A table tag consists of table row tag and table data tag
     Eg: <table>
            <tr><!--1st tr-->
                <td><!--1st tr 1st td-->

                </td>
                <td><!---1st tr 2nd td--><!--CSS For this would be-->

                </td>
            </tr>
            <tr><!--2nd tr-->
                <td><!--2nd tr 1st td-->

                </td>
                <td><!--2nd tr 2nd td-->

                </td>
            </tr>

        </table>
        <style>
                 tr:first-child td:nth-child(2){
                    /*"tr" is 1st child of <table> and "td" is nth-child (i.e., 2) */

                  }
		/*There is only "first-child*, for children after, it is going to be "nth-child{no_of_child}" */
        </style>
	
// Note : <style clear:"both"></style>-->For separating 2 divs.

---

  + selector[:pseudo-class] [::pseudo-element] eg:- a:hover{}, h1::before{}
  + pseudo-class is used to define a special state of an element.
  + pseudo-element is used to style specified parts of an element.
  +  can style HTML elements that have specific attributes or attribute values. a[target_value="_blank"]

---

# Class vs ID
  
   + .className
   + #idName
   + Classes and IDs are more specific than the tags on which they are put.
   + Multiple HTML elements can share the same class, An element can have multiple classes.
   + Value for ID should be unique in the entire HTML document.
   + For including css in html file,
       - We can mad make individual inline styling like,
             
	Eg: <table>
            <tr><!--1st tr-->
                <td style="border-top: 1px solid rgba(158, 156, 156, 0.664); border-right: 1px solid rgba(158, 156, 156, 0.664);"><!--1st tr 1st td-->
                   <!---The above styling is INLINE STYLING--->
                </td>
                <td><!---1st tr 2nd td--><!--CSS For this would be-->

                </td>
            </tr>
            <tr><!--2nd tr-->
                <td><!--2nd tr 1st td-->

                </td>
                <td><!--2nd tr 2nd td-->

                </td>
            </tr>

        </table>

       + We can make internal styling (inside head tag), this style is used for the current 
         (file) webpage internally.

         Eg: <html>
             	<head>
                  	<style>
                         	tr:first-child td:nth-child(2){ /*"tr" is 1st child of <table> and "td" is nth-child (i.e., 2) */
        
                              	border-top: 1px solid rgba(158, 156, 156, 0.664); 
                              	border-right: 1px solid rgba(158, 156, 156, 0.664);
                                     /* <!--1st tr 2st td--> */ 

                                }
                         </style>
				<!---The above styling is called INTERNAL STYLING (specific to the current file)--->
                  </head>
            </html>          

      + We can also create an external stylesheet (Aonther file with ".css" extension) for other 
        file (webpages) to use it (using "link" tag, we can include our stylesheet in html).
           <link rel="stylesheet" type="text/css" href="style.css">

        + Another way to include stylesheet is by adding the below line in html file,
              <style>
                 @import url("style.css");
              </style>

---

# Inline, Internal and External CSS

    + PRIORITY
       + Inline Style (Inside An HTML element)
       + Then Internal Style Sheets (in the head section)
       + Then External
       + Then Browser Default

---

# CSS can do more

   + We can change the element position in the document flow.
   + We can change element size.
   + Font sizing
   + debugging

# Padding, Font size[px, %(browser default + % of it[relative to parent]), em(size of letter 'M', 
  around  16px[relative to parent]), rem(relative to HTML root)] - their quantitative measures

---

# Advance CSS Selectors

   + h1.classname{} //without space.
   + descendant selector(space)
           tr:first-child td:nth-child(2){}; // for the second selector within 1st selector.
   + child selector(>)
       
       <style> 
 
       div>h2{
              font-family: 'Rosario';
         }   // for all h2 elements inside the div tag would have a font-family of "Rosario".
      </style>
   + adjacent sibling selector(+)

    <style> 
 
       div+h2{
              font-family: 'Rosario';
         }   // for all h2 elements(sibling) immediately after the div tag would have a font-family of "Rosario".
      </style>
   + general sibling selector(~)

    <style>

          h2~p{
              color:red; // for all 'p' tag that are sibling(after[within] the h2 tag) of h2 would be "red"	. 
      }




