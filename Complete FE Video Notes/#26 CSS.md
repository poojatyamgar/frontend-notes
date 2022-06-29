---
marp: true
---

# Transitions
       + CSS transitions allows us to change property values smoothly, over a given transition.
            + transition
            + transition-delay
            + transition-duration
            + transition-property
            + transition-timing-function
                  ' Ease (slow, fast, slow)
                  ' Linear (same speed from start to end)
                  ' ease-in (slow start)
                  ' ease-out (slow end)
                  ' ease-in-out (slow - start and end)
                  ' cubic-bezier(n, n, n, n) (lets us define a function in a cubic bezier way)

---

+             div{
               
               width: 100px;
               height: 100px;
               background: red;
               transition: width 2s, height 2s, transform 2s;
               transition-delay: 1s;
               transition-timing-function: linear;

               }

              div:hover{

                 width: 200px;
                 height: 200px;
                 transform: rotate(180deg);
                 }

---

# Animations
       + CSS allows animation of HTML elements without using JS or any other plugin like flash.

         div{
             width: 100px;
             height: 100px;
             background: red;
             position: relative; // to change its position (2)
             animation: myfirst 5s;
             }

         @keyframes myfirst{
             from{background: red;}
             to{background: yellow;}
            }         

         @keyframes myfirst{
             0% {background: red; left:0px; top:0px} // 1st part
             25%{background: yellow; left:200px; top:0px} // 2nd part
             50%{background: blue; left:200px; top:200px;} // 3rd part
             75%{background: green; left:0px; top:200px;} // 4th part
             100%{background: red; left:0px; top:0px;} // 5th part
           }

        + Image overlays

---

        + Image overlays

         .container{
              position: relative;
              width: 200px;
              height: 200px;
              background-color: khaki;
           }

              .overlay{
                  position: absolute;
                  bottom: 100%;
                  left: 0;
                  right: 0;
                  background-color: blue;
                  height: 0;
                  transition: 0.5s;
                 }

               .container:hover .overlay{
                    bottom: 0;
                    height: 100;
                 }

---

# 2D transform

     + With the CSS transform property we can use the following 2D transformation methods:
               + translate()
               + rotate()
               + scaleX()
               + scaleY()
               + scale()
               + skewX()
               + skewY()
               + skew()
               + matrix() // matrix(scaleX(), skewY(), skewX(), scaleY(), translateX(), translateY());	 

           div#div1{
                margin: 100px;
                transform: scale(4,2); //scale(width, height)
             }

           div#div2{
                transform: skew(80deg, 20deg); //skew(x-axis, y-axis)
            } 

---

# 3D transform

     + With the CSS transform property we can use the following 3D transformation methods:    

              +  rotateX()
              + rotateY()
              + rotateZ()
        div{
          animation: rotate3d 4s linear infinite;
          }

---
