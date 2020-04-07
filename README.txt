ITNRO TO HTML:

HTML stands for HyperText Markup Language. (text that can link to other texts)
- made up of tags

homepage always should be name index.html (because of several reasons)

Workspace Folder: (root directory)
    index.html - homepage 
        auto generate DOCTYPE !+tab 
        <!DOCTYPE html> .... </html>

        <head> - is where all the extra information goes 
        <title></title> - the tab title, and the google search information
        <meta></meta> - charset="utf-8" - standar for most language that saves
            save all the character set that we are going to use on the screen.
        

        <body></body> - information in the body tag will show up on the webpage.
        <br> - creates new line (br = break)
        <p></p> paragraph tag - makes new line breaks for us. 
        <em></em> = <i> , but we NEVER use <i> tag! 
        <strong></strong> = <b> the bold tag, but we NEVER use it! 

    css: - cascading stylesheet (the look of ur webpage)
        We use the style="" <- this is called a inline style, avoid USING THIS! 
        We use hexidecimal for the color of the font because we can change the hue of the color.
        font-family changes the text style.
        Stylesheets have a cascading effect. Meaning it affects whatever is in the tag!
        External stylesheet are much easier to make changes. rather then using inline style's

        Example: (btwn stylesheet and inline style)
        compare index.html and page2.html 
        index.html uses the stylesheet and page2.html uses the inline style 
        *** never mix inline and stylesheet ***
        *** always use stylesheets ! ***

        Classes and ID: 
            id - should be unique and only represent one thing (represented by a #idname )
            class - you can have it represent multiple tags (represent by a .classname )
                more common
                you can use it once or use it multiple times rather than using id. 
        

Box Model:
    Maring: 
        If the margin property has one value: margin: 25px; 
        all four margins are 25px
        Margin creates space outside of the container.
    Border: 
        3 properties: 
            border-width: border-left-wdith: border-right-width:
            border-color: border-left-color: border-right-color:
            border-style:
        Order of styles matter

    Padding:
        Creates an empty space with the background color
        Creates space inside of your container. 

    Order is always: margin boarder padding box (out to in)
        or just do inspect

Background Imgs: (the more padding you have, the more background you have)
    background-repeat: where and how you want it to repeat or   
        if you don't want it to repeat.
            repeat-x;
            repeat-y;
            no-repeat;
            round;
    background-size:
        auto; - is default
        contains; - you can see the entire image (but it will repeat if there is empty space)
        cover; - covers the entire div! so it grows or shrink porpotionally
                    does not repeat itself!
                    ***becareful of the padding tho, because it will stretch your image***
    background-position:
        top-left; - this is the default.
        center; - center's the picture 
        right-bottom - readjust the picture the picture. 

Styling Text:
    font-size: 70px; - sizing of your fonts
    font-family: sans-serif; - the style of your fonts (these are depending on what computer you have)
        some systems like mac don't have Calibri; 
        Futura; is a mac font style, but PC's don't have it. 
        ***to stop this from happening you can do a system stack***
        ****basically the comma is a system stack, it keeps loading the next font style *****

        font-family: Futura, sans-serif;
        Link - http://wwww.cssfontstack.com - tell you what font on computer runs on.

        font-style: oblique; // fake italic
        font-style: italic; 

        font-weight: bolder; //one size up from what your font weight is. 
        font-weight: bold; //doesn't matter it'll just be bold
        font-wieght: lighter; //once size down from what your font weight is. 

        if font is more than one word, put them in quotes like this: 'Times New Roman','Segoe UI',...etc

        *** all text have margin top and margin bottom. They are automatically applied when you create them***
        Spacing: all h1, p, have automatic spacings. To adjust this we use the margin element.
            margin-top: 0px; 
            margin-bottom: 0px; 

            Space between your lines - 
                line-height: 40px; //equally distributes the line height to the top and bottom. 
                    therefore 20px to the top and 20 to the bottom.
                    DON'T USE px. use the bottom vvvvvvvvvvvv
                    ****Using line-height: wiht a number; basically applies to your spacing depending on your
                    font-size, it equally distributes it to the top and bottom.
                line-height: 1; // line height of 1 makes it equal to your font-size:
                line-height: 1.4; // these numbers applies to your spacing depending on your font-size. 
                line-height: 2; //basically is a double space. 

        text-align: left; right;

        text-decoration: line-through;
        text-decoration: underline;
        text-decoraton: overline; 
        text-decoration: none; //removes features
        
        text-transform: capitalize; lowercase; none; uppercase;
            capitalize - only caps the first letter of each word. 
            uppercase - every letter is uppercase. 
            
    color: #3747b3;

Styling Links
    you have to manual style them, even though they are inside of a tag
    the browser has its own default blue for them. To do so:

    a{
        color: black;
    }

    Sudo class of a, hover, is when the mouse goes over on top.
    you can apply any type of feature to it so when you hover your mouse over it. 
    it takes affect.

    Links have to be in this order!: link, visited, hover, active

    //default 
    a:link{
        color: black;
    }

    links that you HAVE clicked on
    a:visited{
        color: pink; 
    }

    a:hover{ 
        color: yellow;
        font-size: 50px; 
        font-family: sans-serif;
    }

    when you click and hold onto the link. 
    a:active{
        color: blue;
    }

    ****can also do a:focus
    a:focus allows the user to tab cycle through all the links on the webpage
        so it takes affect to a link that when you tab thorugh your website
        it is a keyboard acessability feature.
    a:hover,
    a:focus{
        color: aqua;
    }

CSS selectors!
    the last selectors in your css stylesheet always takes affect.
    so if you edit a p tag at the top of the stylesheet and you edit it again
    at the bottom. The bottom p tag selector takes affect OVER the top one. 

    .body-text{
        backgoroudn-color:: #79acd1;
        padding: 50px;
    }

    selects the div class name , and specifically get the p tags in THAT CLASS! 
    .body-text p {
        color:white;
    }
    .body-text a{
        color: #f7c0f4;
    }

    .body-text a:hover{
        color: #DDD;
    }

    specificity calculator!
        even though you have a link that is an important link class,
        the .body-text a{} will always take affect bc of the specificity number
            classses = 10pts and a tags = 1pt. 
    .important-link{
        color: yellow;
    }

    if you really want it to take affect then we can do this! 
    .important-link,
    .body-text .important-link{
        color: yellow;
    }

    OVERULE MEHOTD: by using the !important keyword
    .important-link{
        color: yellow !important; //only use this if this is the LAST RESORT! do not abuse this. 
    }

HTML List
    ordered List: is a numbered list
        <ol>
            <li>Item Number 1</li>  // List Item = li
            <li>Item Number 2</li>
            <li>Item Number 3</li>
            <li>Item Number 4</li>
        </ol>

        CSS style
            
            ol{
                list-style-type: upper-roman; //instead of numbers becomes uppercase roman numerals
                list-style-type: upper-alpha;
            }
    
    Under Ordered List: is a bullet list
        <ul>
            <li>Item Number 1</li>  // List Item = li
            <li>Item Number 2</li>
            <li>Item Number 3</li>
            <li>Item Number 4</li>
        </ul>

        CSS Stylesheets
            body{
                text-align: center;
            }


            ul{
                list-style-type: circle; square; disk; none;
                list-style-image: url(../img/icon.png); //becareful when using this, it will take the icon at FULL size.
                background-color: pink;
                padding: 50px;
                list-style-position: inside; //takes in the bullet points so when we center or move the text inside of the text , it goes with it
            }

            edit the ul links specifically.
            ul li{
                background: red;
                margin: 5px; margin-bottom: 15px;
            }

Floats & Clears
    img{

        There is not float: center option! 

        float: left; // moves the picture to the left side of webpage
        float: right; 
        float: none; //default 
        margin-right; 20px; // pushes the text away from the img if u float left
    }

    .red-box{
        height: 500px;
        width: 500px;
        background: rgba(255, 0, 0, .5);
    }

    .blue-box{
        height: 400px;
        width 700px;
        background: blue;
    }

    p{
        clear: both; // have the text no wrap around imgs
    }

    clear:both, always forces a new line! only works with float:
    clear:right; focuses things that float to the right
    clear:left; focuses things that float to the left.



Colors in CSS
    HEX, RGB, and HSL

    hexidecimal
        background: #RRGGBB values , scale from 0->9 A->F
            example - background: #FFFFFF; = white
                      background: #000000; = black
                      background: #8fdb83; = light green

    RGB values
        background: rgb(143, 219, 131); = light green as well 
        
        rgba - a stands for alpha, the transparency, values are from 0 to 1
        red green blue alpha 

        background: rgba(255, 0, 0, 0.5); = the .5 means 50% opacity, 
            the higher the a number is the less transparency it will be. 

        if you use rgb you can also adjust the opacity by using:
        opacity: 0-1; //values are from 0 to 1. 

    HSL
        stands for: Hue Saturation Lightness
        the lower the saturation, the more grey the color will look
        Lightness = 0% is black 100% white
        background: hsl(360, 100%, 50%);
        if you add the a into hsla = a is the same for rgba so it manages the opacity.


        


File organization:
       *** very important when creating a web design.***
       *** always name thing lowercase for folder names ***
       *** try to be very specific when naming your files ***
       *** avoid spaces in all files! ***
        img folder. (sub directory) images
        css folder (sub directory) stylesheet
        js folder (sub directory) javascript


SHORTCUTS AUTO generate in VSC:
!+tab
p+enter
.div-class-name
p.p-class-name

