---
marp: true
---

# FONTS
    + font-style
    + font-variant
    + font-weight
    + font-size : 2vw (responsive font based on screen size.)
    + line-height : gives sapce above and below words. 
    + font-family : font1(browser tries rendering it), font2(fallback to render it, if in case 
      font1   does not render.), font3
    + font(-short_hand-) : font-style font-variant font-weight font-size line-height font-family
                     Eg  : italic small-caps bold 12px/30px Georgia, serif;
    + Web safe fonts
    + Text-decoration : none (-when we do not want underline for our links-)

  ## Comment in css: (short-cut)- "ctrl+power(^)+/"

---

# CSS Properties
    + background-image : linear-gradient(direction, color-stop1, color-stop2, ...);
      Eg : body{
           background-image : linear-gradient(red, yellow, blue) 
           } result would be a (top-bottom) gradient(colors sahading from mentioned 3)
           OR
           body{
           background-image : linear-gradient(to right, right, yellow, blue)
           } result would be a (left-right) gradient (colors shading from mentioned 3)
    + background-image : radial-gradient(bisque, aqua, white)
      result would be circular effect of colors. 
    + hr{ width:50%}result would be a horizontal line taking about 50% of where it is present.
    + Text shadow
    + Box shadow

---

# CSS Selectors And Properties
    + Element
    + ID // "#idName{}"
    + Class // ".className{}"
    + Universal *
    + Group - h1, h2, p{
               text-align : center;
               color : red;
              }

---
