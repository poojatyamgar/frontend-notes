---
marp: true
---

# CSS Positioning Systems

     + Position:
       + Static (default)
       + Relative (position based on parent)[small margin at the top and left]
            The element is going to move around based on itself within its parent.
            Relative doesn't mean the entire browser width. 
            The space secured for that element will not be threatened at all when we put position=relative.
       + Absolute (It positions according to parent[relative])
       + Fixed (It gets fixed to position [as we scroll though it remains fixed]) 
       + Sticky  
            Similar to position fixed, but we can achieve a relative positioning on your browser unless we scroll down,
            unless it becomes fixed and sticky to the browser position.
            However, at scrolling it becomes fixed at its place.
            Sticky, is used because "relative" positioning has the main merit of keeping the space of that element secured, so that the document flow does not change
               which changing the position of that particular element.

---

     + Text-align: center; // manipulate the text within the parent
          It can be used for all elements, for which "width" is not defined.

     + Margin: 
        + auto;
           It can be used for all elements, for which "width" is defined, but still need to be "center".
        + initial
        + inherit
        + unset

---

     + Display: 
       + Block (All contents inside a block)
       + Inline (All elements are inline[same line])
       + inline-block (All elements are block-inline)
       + none (to hide, [element vanish from display])
     
      "div" tag has block display.
      "span" tag has inline display.

---

     + Visibility:
        + hidden 
           similar to "display: none", but here it shows the description while inspecting it.
        + collapse
        + visible
        + initial
        + inherit
        + unset

---
