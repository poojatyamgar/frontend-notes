---
marp: true
---

## Responsive Web Design

#### A responsive website:-

+ Any wesite design to adapt its layout to the viewing    environment of  different devices in different browser sizes,
   By using fluid propotion based grids, flexible images, CSS free media query etc.

+ Site layout adapts to the size of the device.
    + One way to achieve this is to have different websites for each device.
    + We can have a fluid design(changes in a smooth fashion) which fits to large screen as well as small screen, we can use a grid system.

---

#### Grid System:-

+ 12 column Grid Responsive(Customize based on screen size) Layout, (the number 12 is used because it's a composite number, which can be divided into even and odd parts as per the screeen size.)
+ It uses a '%' of browser width.
+ These can be *nested* - one of the grids can have its own 12 column grid.

### Note :-

+ Can select element based on attribute selector, in CSS. 

      <style>
        [class*="col-"]{
            background-color: fuchsia;
        }
        </style>

---

#### Flexbox:-

+ The flexible Box Layout makes it easier to design flexible responsive layout structure without using float or positioning.

+ The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.

+ **Refer, mdn docs for "Basic Concepts Of Flexbox"** , to know to use the flexbox layout of CSS.

---

    <html>
    <style>
        .flex-container{
            display:flex;
        }
        div{
            height: 500px;
            background-color: lightblue;
            border: 1px solid blue;
        }
    </style>
    <body>
        <div class="flex-container">
            <div style="order:1; flex-grow:1;">1</div>
            <div style="order:3; flex-grow:1;">2</div>
            <div style="order:2; flex-grow:8;">3</div>
        </div>
    </body>
    </html>

---

#### Media Queries:-

+ The media tag "@media" was used earlier to find which media is browsing your webpage.
   Lets say the media could be "screen/printer,etc.," so the respective layout to be shown to the user or printer.
   This way to judge the kind of media which is trying to access the webpage, the media tag was used.
   Later On,

+ Media query can be used to check:
  + width and height of viewport.
  + width and height of device.
  + orientation (landscape or portrait).
  + resolution. 

---

#### Viewport:-

+ The viewport is the size of the browser from left to right and top to bottom.

+ Popular technique for delivering a tailored stylesheet to desktop, laptop, tablet, and mobile phones.


---
    <html>
    <style>
        /* [class*="col-"]{
            background-color: fuchsia;
        } */
        .column{
            width:25%;
        }

        @media screen and (max-width: 992px){
            .column{
                width: 50%;
            }
        }

        @media screen and (max-width: 600px){
            .column{
                width: 100%;
            }
        }

        @media screen and (max-width: 600px){
            div.onbigscreenonly{
                display:none;
            }
        }

        div{
            float: left;
            box-sizing: border-box;
            height: 500px;
            background-color: lightblue;
            border: 1px solid blue;
        }

        div.onbigscreenonly{
            background-color: fuchsia;
        }

    </style>
    <body>
        <div class="column"></div>
        <div class="column"></div>
        <div class="column"></div>
        <div class="column onbigscreenonly"></div>
    </body>
    </html>

---

