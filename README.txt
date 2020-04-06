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

