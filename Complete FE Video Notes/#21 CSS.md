---
marp: true
---

# The 'BOX model'

      + Margin
      + Border
      + Padding
      + Content
      + Padding
      + Border
      + Margin
   + For 2 elements - Top and bottom margins overlap, the margins don't add. The larger margin wins.
   + http://markusvogl.com/web1/interactive_box_model/css_box_demo.html

---

# Box Sizing

    + box-sizing: content-box(parent)/border-box(child)
    + Box sizing is not an inherited property.
    + Can use * selector for applying box sizing type to all.
 + https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing
    + margin: 25px 30px 35px 40px //(top right bottom left)
      margin: 25px(top,bottom) 30px(right,left)
      margin: 25px(top) 30px(right,left) 35px(bottom)

---

# Outline

   + It is not a part of the element.
   + May overlap other elements.
            + Outline
            + Margin
            + Border
            + Content
 
---

# Overflow

    + If a content (box-sizing: content-box) doesn't fit in a size, that's where Overflow comes in.  
    + overflow, overflow-x(horizontal), overflow-y(vertical):
              + visible - default (outside box the content will be visible)
              + hidden (outside box content will be hidden[invisible])
              + scroll (outside box content will be accessible via a scroll [for both horizontal 
                and  vertical] )
              + auto (preferred, adds scroll bar only when it is necessary [based on a and y axis])

---

# CSS sizing methods

    + px
    + pt(Eg:- 72pt means 1 inch of page) 
    + em(relative type of sizing to parent[parents parent])
    + rem(relative to size of 'M' (html root))
    + vw(viewport width)[size of browser, and with screen)
        With resizing of browser, the font-size will resize accordinly, will lead to a good user-experience.
    + % (relative sizing based on parent)
