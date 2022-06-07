---
marp: true
---

# Z - Index

    + Children sit on top of parents.
    + It only works with positioned elements.

          + position: relative;
            z-index : 1;
          + position: absolute;
            z-index : -1;
    + Setting position and position in the html flow affects which element will be on the top 
      of  another. 
    + When no z-index is applied:
          + Root element(the <html> element)
          + Non-positioned elements in the order they are defined.
          + Positioned elements in the order they are defined.
    + When applying certain CSS properties, an element can form a stacking context 
      (Eg: being   transparent)
      
      Z-index values only have a meaning within the same stacking context.

