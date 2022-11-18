Viewport
<meta name="viewport" content="width=device-width,initial-scale=1.0">

media queries
in head
@media(min-width:600px){
body{
 background-colour:red;
}
}


Flexbox

#idname{
display: flex'
flex-wrap: wrap;
}

Grid
#grid{
background:color: green;
display: grid;
padding: 20px;
grid-column-gap: 20px;
grid-row-gap:10px;
grid-template-columns: 200px 200px auto;
}

Bootstrap -> Popular CSS library

<link rel="stylesheet" href ="<link from google[lol]>">

Bootstrap column model

<div class="col-lg-3 col-sm-6">
  This is section
</div>

large screen - 3 units
small screen -6 units

Sass is a lanuage that is essentially an extension to css

for sass file name xyz.scss

$color:red;
ul{
 font-size:14px;
 color: $color;
}
ol{
font-size:18px;
color: $color;
}
chrome and safari cant understand scss
so compile scss to css
install sass
in cmd sass xyz.scss: xyz.css
in sass
we can nest
div{
font-size: 18px;
p{
color: blue;
}
}

sass can also provides inheritance

%msg{
font-family: arial;
font-size: 18px;
font-weight: bold;
border: 1px solid black;
padding: 20px;
margin: 20px;
}

.success{
@extend %msg;
background:color: green;
}

## HTML

<code>&lt; form action="xyz..html" method="GET" &gt; </code>
<label for="name">Name</label>
<input name="name,email,number" id="name" placeholder="Enter Name" value= " xyz" required min="1" max="200 for number AND DATE type" step='5'>
or
<label>
   Password
   <input name="password">
</label>

CHECKBOX for all'
RADIO for one
<div>
<label for="male">Male</label>
<input type="radio" name="gender" id="male" value="male"> 
</div>
<div>
<label for="Female">FeMale</label>
<input type="radio" name="gender" id="Female" value="female"> 
</div>

<label for="eyecolor" >Eye Color</label>
<select name="eyecolor" id="eyecolor" multiple>
<option value="Green">Green</option>
<option value="Red">Red</option>
</select>
<textarea id="bio" name="bio" rows="10"></textarea>

## CSS

-> text-decoration: overline;
                               line-through

-> box-sizing: content-box;
                        border-box;


-> font : inherit;

-> text-transform :  lowercase;

-> text -align : left;
                      : justify;

-> text-indent: 2em;

-> line-height : 1.5;

-> word-spacing: 0.5 em;

-> font-weight: 300,bold,bolder;

-> font-style : italic;

->font-family : sans-serif, monospace ; (" double quotes for 2 or more words in the family")


## Links

-> text-decoration: none;
-> cursor: not-allowed;
                 pointer


a:visited : {               -> visited is pesudo class  that means it represents the current state
}
a:hover{

}

a:active{

}

a:focus{   -> accesed through tab

}


## List 

ol{
      list-style-type: decimal;
                              disc;
                              circle;
                              upper-roman;
                              none;
}

<code> &lt; ol start="5" reversed &gt;  </code>


text-align : center;
list-style-position: outside;

color: blue; -> affects all
line-height: 1.6; affect all
list-style-image: url(" ")

list-style : square url(" ") inside;


ul li:nth-child(odd,2,even){
color: red;
}

::marker{
color : red;
content: "only 5$>>";
}



 display: block;
 li: last-child a {
 border-radius : 0 0 2rem 2rem;
 }

inline

Displays an element as an inline element (like <span></span>). Any height and width properties will have no effect

for inline elements , cant add width, height or margin
when needed to used that we use inline-block

block

Displays an element as a block element (like <p></p>). It starts on a new line, and takes up the whole width

inline-block

Displays an element as an inline-level block container. The element itself is formatted as an inline element, but you can apply height and width values


## FLOATS

 float: left;     for the float element
 can add margin and padding

clear: left,right,both;
overflow: auto; for the container element


## COLUMN

column-count : 4;
column-width: 250px;
columns: 4 250px;
column-rule: 3px solid black;
column-gap: 3rem;

Margin Collapsing

break-inside: avoid;



## POSITION


static position default

position: absolute takes the closest relative to top and bottom if not present takes the window as relative

relative : relative to parent container even if it is not relative

fixed : it is fixed even if you scroll down or up position acc. to the window 

z-index: 1;

sticky : sticks to the page till given top and bottom


