# css-silicium

## HTML used to create a skelton of webpage but CSS style our webpage
 
---

**There are many ways to style our elements:**
1. inline css
    + Example:
    ```
    <h1 style="background-color: red;">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Obcaecati, magnam?</h1>
    ```
> In directory 1>1.1>index.html , we used this format.

2. using style tag in html file
    + We shoud use tag style with attribute type="text/css"
    + Example:
    ```
    <head>
        <style>
            h1{
                background-color: red;
            }
            p{
                color: red;
            }
        </style>
    </head>
    <body>
        <h1>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Obcaecati, magnam?</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti soluta dolor fuga! Culpa voluptatem, quibusdam perferendis dolor vel ipsum. Tempora temporibus quibusdam corporis totam repudiandae minima nemo voluptatibus distinctio assumenda!</p>
        <h1>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Obcaecati, magnam?</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti soluta dolor fuga! Culpa voluptatem, quibusdam perferendis dolor vel ipsum. Tempora temporibus quibusdam corporis totam repudiandae minima nemo voluptatibus distinctio assumenda!</p>
    </body>
    ```
> In directory 1>1.2>index.html , we used this format.

3. External CSS file
    + To do this method , create a file for example "style.css" , then by link tag , connect that css file to html file
        + To this method we use link tag , with rel="stylesheet" and href="address_css_file.css"
    + Example:
    ```
    <!-- HTML File -->
    <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>CSS tuturial</title>
    <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <h1>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Obcaecati, magnam?</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti soluta dolor fuga! Culpa voluptatem, quibusdam perferendis dolor vel ipsum. Tempora temporibus quibusdam corporis totam repudiandae minima nemo voluptatibus distinctio assumenda!</p>
        <h1>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Obcaecati, magnam?</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti soluta dolor fuga! Culpa voluptatem, quibusdam perferendis dolor vel ipsum. Tempora temporibus quibusdam corporis totam repudiandae minima nemo voluptatibus distinctio assumenda!</p>
    </body>
    ```
    ```
    /* CSS File */
    h1{
        background-color: red;
    }
    p{
        color: red;
    }
    ```
> In directory 1>1.3>index.html & style.css , we used this format.

---

**To specify an element(s) in css , we can use id or class .**
1. use id
    + With id , we can specify just one tag
    + To use id , we should specify id with sharp(#) 
        + For example: #id
    + Example:
    ```
    <!-- HTML File -->
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <title>CSS</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <h1 id="first-h1">Title 1</h1>
        <p id="first-p">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa voluptates recusandae commodi obcaecati excepturi, sapiente adipisci fugiat dolore corporis cumque officiis quam ut aliquam maiores? Iure accusamus natus autem veritatis.</p>
        
        <h1>Title 2</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa voluptates recusandae commodi obcaecati excepturi, sapiente adipisci fugiat dolore corporis cumque officiis quam ut aliquam maiores? Iure accusamus natus autem veritatis.</p>
    </body>
    ```
    ```
    /* CSS File */
    #first-h1{
        background-color: red;
    }

    #first-p {
        color: red;
    }
    ```
> In directory 2>2.1>index.html & style.css , we used id for styling.

**We should not use id for more than one element . To do this work , we should use classes .**

2. use class
    + With class , we can specify one or more tag(s) .
    + To use id , we should specify id with dot(.) 
        + For example: .class
    + Example:
    ```
    <!-- HTML File -->
    <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>CSS</title>
    <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <h1>Title 1</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa voluptates recusandae commodi obcaecati excepturi, sapiente adipisci fugiat dolore corporis cumque officiis quam ut aliquam maiores? Iure accusamus natus autem veritatis.</p>
        
        <h1 class="bg-red">Title 2</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa voluptates recusandae commodi obcaecati excepturi, sapiente adipisci fugiat dolore corporis cumque officiis quam ut aliquam maiores? Iure accusamus natus autem veritatis.</p>

        <h1>Title 3</h1>
        <p class="bg-red">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa voluptates recusandae commodi obcaecati excepturi, sapiente adipisci fugiat dolore corporis cumque officiis quam ut aliquam maiores? Iure accusamus natus autem veritatis.</p>
        
        <h1 class="bg-red">Title 4</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa voluptates recusandae commodi obcaecati excepturi, sapiente adipisci fugiat dolore corporis cumque officiis quam ut aliquam maiores? Iure accusamus natus autem veritatis.</p>
    </body>
    ```
    ```
    /* CSS File */
    .bg-red{
        background-color: red;
    }
    ```
> In directory 2>2.2>index.html & style.css , we used class for styling.

---

**To use rgb color we can use this format**
+ Example:
```
/* CSS File */
.bg-color{
    background-color: #ff7878;
}
#first-p{
    color: #75fc75;
}
```
+ First 2 number is for red , second 2 number for green and third 2 number for blue

> In directory 3>index.html & style.css , we used this color.

---

**Note : If we use a style for a parent element , it will change style of childs element**
    + For example : if we change style of body tag , it will change style of childs tags .

---

**Text properties in css :**
1. font-family
    + With font-family property , we can change font-family of element
    + for Example : font-family : tahoma;
2. font-size
    + With font-size property , we can change font-size of element
    + for Example : font-size : 18px;
3. text-align
    + With text-align property , we can change align of text
    + Values of text-align:
        1. text-align: left;
            + Used for left to right language like English websites.
        2. text-align: right;
            + Used for left to right language like Persian websites.
        3. text-align: justify;
            + Used for to justify out text .

---

**Specific selector in CSS :**

*To specify span in li and li in ol , we should say :*
```
ol li span {
    /* CSS Code */
}
```
*We can specify which chid get the style , we can use psedu classes like : element:first-child , element:last-child , element:nth-child(odd) , element:nth-child(even) , element:nth-child(3n+2) and so on*


> In directory 4>index.html & style.css , we used these selectors.

---

**In this part , we want to explain about link states . Then we learn how to style links .**

*There are many types of link state :*
1. Default:
    + Example:
    ```
    .link{
        /* CSS code */
    }
    ```
2. hover
    + Example:
    ```
    .link:hover{
        /* CSS code */
    }
    ```
3. active
    + Example:
    ```
    .link:active{
        /* CSS code */
    }
    ```
4. visited
    + Example:
    ```
    .link:visited{
        /* CSS code */
    }
    ```
> In directory 5>index.html & style.css , we used these link states.

---

**If we want to change a property with transition , we can use transition property.**
+ Example:
    ```
    /* CSS File */
    /* Default state */
    .google{
        background-color: black;
        transition: background-color 0.5s; 
    }

    /* When hover the link */
    .google:hover{
        background-color: red;
    }

    /* When your mouse click in link(not release the mouse) */
    .google:active{
        background-color: aqua;
    }
    ```
> In directory 6>index.html & style.css , we used transition.

---

**Here are the important properties of css :**

1. width:
    + Explain: This property set width of element
        + Example 1: [Fixed size with pixel(px)]
        ```
        /* CSS code */
        width: 200px;
        ```
        + Example 2: [Relative size with percentage(%)]
        ```
        /* CSS code */
        width: 25%px;
        ```
2. height
    + Explain: This property set height of element
        + Example 1: [Fixed size with pixel(px)]
        ```
        /* CSS code */
        height: 600px;
        ```
        + Example 2: [Relative size with percentage(%)]
        ```
        /* CSS code */
        height: 50%px;
        ```
3. float
    + Explain: This property allows us to put elements near of each other
    + Values of float :
        1. float : left;
        2. float : right;

4. border
    + Explain: This property create border for element
    + Example:
    ```
    border: 1px solid black;
    ```
    + We can set type of the border like :
        1. solid
        2. dashed
        3. dotted
        4. ridge
        5. double

5. clear
    + Explain: This property clear erea left or right or both of the element 
    + Values of float :
        1. clear : left;
        2. clear : right;
        3. clear : both;

**Important About CSS padding !**
**Each element have some spaces :**
+ Content
+ Padding
+ Border
+ Outline
+ Margin

*So with box-sizing property , we can say calculate border from content or border*

6. box-sizing
    + Explain: This property say that from where to calculate element dimention(link width or height)
    + Values of box-sizing :
        1. box-sizing : content-box; (default)
        2. box-sizing : border-box;

7. padding
    + Explain: This property say that how mush padding between content and border
    + Types of set value for padding :
        1. padding : 10px;
            + When we set padding like this , padding apply 10px from left, right , top and bottom
        2. padding : 10px 30px;
            + + When we set padding like this , padding apply 10px from top and bottom , 30px from left and right
    + We can set padding from each position like :
        1. padding-left : 10px;
        2. padding-right : 20px;
        3. padding-top : 30px;
        4. padding-bottom : 40px;

8. margin
    + Explain: This property say how much margin between two border
    + Types of set value for margin :
        1. margin : 10px;
            + When we set margin like this , margin apply 10px from left, right , top and bottom
        2. margin : 10px 30px;
            + + When we set margin like this , margin apply 10px from top and bottom , 30px from left and right
    + We can set margin from each position like :
        1. margin-left : 10px;
        2. margin-right : 20px;
        3. margin-top : 30px;
        4. margin-bottom : 40px;
    + Note: If "box-sizing : border-box ;" , this will not apply sizing from margin !
    + Important note : When we set "margin: auto;" means that place element middle . (See example in directory 8)

9. border-radius
    + This property say how mush radius from border
    + Example:
        1. border-radius:30px;
        2. border-radius:30%;
    + If we want border from top-left,top-right, bottom-right and bottom-left , we can set border-radius like :
        + border-radius: 10px 20px 30px 40px;

10. box-shadow
    + First value is the horizontal offset of the shadow. A positive value puts the shadow on the right side of the box, a negative value puts the shadow on the left side of the box
    + Second value is the vertical offset of the shadow. A positive value puts the shadow below the box, a negative value puts the shadow above the box
    + Third value is the blur radius. The higher the number, the more blurred the shadow will be 	
    + Forth value is the spread radius. A positive value increases the size of the shadow, a negative value decreases the size of the shadow
    + Fifth value is the color of the shadow. The default value is the text color. Look at CSS Color Values for a complete list of possible color values.
    + If first and second value is 0 , it means highlight the element
    + Example : box-shadow: 10px 10px 8px 1px gray;

11. cursor
    + Explain: We can change cursor pointer when our mouse on the element
    + Example: cursor: pointer;

12. overflow
    + Explain: We can set overflow when an element overflow from that element
    + Values of overflow:
        1. overflow:hidden;
            + It means ignore overflow values
        2. overflow:auto;
            + It means scroll overflow values

**We can set before and after element add some elements with content property**
    + element:before
    + element:after

13. content
    + Example:
        + In this example we want to send footer to newline
    ```
    main:after{
        content : " ";
        display : block;
        clear: both;
    }
    ``` 

14. display
    + Explain: Some tags like div,h1 to h6 , p and so on have display: block ;(default) . But some other tags like span , b , i and so on have display: inline; (default). But we can change display of elements with display property .
    + values of display:
        1. display : block;
        2. display : inline;
        3. display : inline-block;
            + Some property like width can not set for inline elements , so we should use inline-block for this elements.
            + Example:
            ```
            span{
                width: 100px;
                background-color: red;
                display: inline-block;
                text-align: center;
            }
            ```
> In directory 7>index.html & style.css , we used properties.

---

**To style to more than one element we can use comma(,) between elements .**
+ Example:
    ```
    input, texterea{
        /* CSS code */
    }
    ```
15. line-height
    + The line-height property specifies the height of a line. (More used in text input or texterea)
    + Example : line-height:30px;

*We can set when click to input or texterea , change for example background color*
+ Example:
    ```
    input[type="text"]:focus ,input[type="password"]:focus , textarea:focus{
        background-color: rgba(161, 227, 155, 0.848);
    }
    ```
16. outline
    + The space between border and margin is ouline 
    + Example: ouline: 0px;

17. position
    + With position property , we can change position of the element with **left, right, top and bottom** property
    + values of position
        1. position : relative ;
            + With this position value we can change position from its normal position.
            + Example:
            ```
            .position{
                position: relative;
                left: 30px;
                top : 160px;
            }
            ```
        
        2. position : absolute ;
            + With this position value we can change position from main window.
            + Example:
            ```
            .position2{
                position: absolute;
                left: 0px;
                top : 0px;
            }
            ```
            + **Important note : If we want to set position of element for example top and left parent element , we should set position parent to relative**

        3. position : fixed;
            + With this position we can change position **always** from the window 
            + Example:
            ```
            .position3{
                position: fixed;
                right : 0px;
                bottom : 0px;
            } 
            ```
> In directory 8>index.html & style.css , we used properties.

---

## Flex Box

**By default , when we use "display :flex;" for our tag , child elements display near of each others.**
+ Example:
    ```
    main{
        display:flex;
    }
    ```

**Properties of flex box are :**
1. flex-direction
    + This property shows how to put elements near of each others.
    + Values of flex-direction
        1. flex-direction : row;(default)
        2. flex-direction : row-reverse;
        3. flex-direction : column;
        4. flex-direction : column-reverse;

*Note : if flex box element can not put near of each others , flex box minimize width of each element to can put elements near of each other*

2. flex-wrap
    + This property shows that how flex box put near of each others when there is no space.
    + Values of flex-wrap
        1. flex-wrap : nowrap;(default)
            + This value for flex-wrap shows that reduce elements flexible .
        2. flex-wrap : wrap;
        3. flex-wrap : wrap-reverse;

**Note : if we want to elements of flex box use display: flex; we should add "display:flex;" for elements .**

3. justify-content
    + This property shows that how to put elements of flex box in row
    + Example : (To centerlize elements in row)
    ```
    justify-content : center;
    ```

4. align-items
    + This property shows that how to put elements of flex box in column
    + Example : (To centerlize elements in column)
    ```
    justify-content : center;
    ```
> In directory 9>index.html & style.css , we used properties of flex box.