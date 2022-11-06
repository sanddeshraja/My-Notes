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

