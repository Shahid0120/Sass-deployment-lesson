# Tuesday Notes
https://sass-lang.com/guide
# # Sass
Mapping allows to see the the scss stuff from the web (preference--> source maps)

# ## how to link 
@ import allwos to link partials with the file _ i.e _home.scss
ie. @import "partials/home.scss";

### using the & 
this is used for nesting within nesting  --> this serves as the main purpose of scss
ei.g 
 body {
     p {
         &:hover {

         }
     }
 }

## adding variables:
    using hotkeys $ 

### using mixin
this is more for general use og a group of things
ie 
@mixin background-color {
    background-color: black;
    color: red;
}

header {
    @include background-color();
}
--> This chanegs the colour by putting $
footer {
    @include background-color($color:green)
}


### inheritence
This is more for specialised times like an id
%msg-shared {
    border: 2px solid black;
    font-size: 30px;
    font-style: italic;
}

.sucess {
    @ extend %msg-shared;
    color: green;
}


### naming partials
All partials files need to have:
     _name.scss 


