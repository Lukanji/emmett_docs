# Emmet Documentation

## Syntax

### Child: >

```html
nav>ul>li

<nav>
  <ul>
    <li></li>
  </ul>
</nav>
```

### Sibling: +

```html
div+p+bq

<div></div>
<p></p>
<blockquote></blockquote>
```

### Clim-up: ^

```html
div+div>span+em^bq

<div></div>
<div><span></span><em></em></div>
<blockquote></blockquote>
```

### Grouping: ()

```html
div>(header>ul>li*2>a)+footer>p

<div>
  <header>
    <ul>
      <li><a href=""></a></li>
      <li><a href=""></a></li>
    </ul>
  </header>
  <footer>
    <p></p>
  </footer>
</div>
```

### Multiplication: \*

```html
ul>li*5

<ul>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

### Item numbering: $

```html
ul>li.item.$*5

<ul>
  <li class="item 1"></li>
  <li class="item 2"></li>
  <li class="item 3"></li>
  <li class="item 4"></li>
  <li class="item 5"></li>
</ul>
```

### ID and CLASS attributes

```html
#header
<div id="header"></div>

.title
<div class="title"></div>

form#search.wide
<form action="" id="search" class="wide"></form>

p.class1.class2.class3
<p class="class1 class2 class3"></p>
```

### Custom attributes

```html
p[title="Hello world"]
<p title="Hello world"></p>

td[rowspan=2 colspan=3 title]
<td rowspan="2" colspan="3" title=""></td>

[a='value1' b="value2"]
<div a="value1" b="value2"></div>
```

### Text: {}

```html
a{Click Me}
<a href="">Click Me</a>

p>{Click}+a{here}+{to continue}
<p>Click<a href="">here</a>to continue</p>
```

### Implict tag names

### HTML

```html
footer
<footer></footer>

!
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
 
</body>
</html>

a
<a href=""></a>

a:link
<a href="http://"></a>

a:mail
<a href="mailto:"></a>

abbr
<abbr title=""></abbr>

acronym, acr
<acronym title=""></acronym>

base
<base href="">

basefont
<basefont>

br
<br>

frame
<frame>

hr
<hr>

bdo
<bdo dir=""></bdo>

bdo:r
<bdo dir="rtl"></bdo>

 bdo:l
<bdo dir="ltr"></bdo>
 
 col
 <col/>

 link
<link rel="stylesheet" href="">

link:css
<link rel="stylesheet" href="style.css">

link:print
<link rel="stylesheet" href="print.css" media="print">

link:favicon
<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">

link:touch
<link rel="apple-touch-icon" href="favicon.png">

link:rss
<link rel="alternate" href="rss.xml" type="application/rss+xml" title="RSS">

link:atom
<link rel="alternate" href="atom.xml" type="application/atom+xml" title="Atom">

link:import, link:im
<link rel="import" href="component.html">

meta
    <meta>

meta:utf
<meta http-equiv="Content-Type" content="text/html;charset=UTF-8">

meta:vp
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

meta:compat
    <meta http-equiv="X-UA-Compatible" content="IE=7">

style
    <style></style>

script
    <script></script>

script:src
<script src=""></script>

img
<img src="" alt="">

img:srcset, img:s
<img src="" alt="" srcset="">

img:sizes, img:z
    <img src="" alt="" sizes="" srcset="">

picture
<picture></picture>

source, src
    <source>

source:src, src:sc
<source src="" type="">

source:srcset, src:s
<source srcset="">

source:media, src:m
<source media="(min-width: )" srcset="">

source:type, src:t
<source srcset="" type="image/">

source:sizes, src:z
<source sizes="" srcset="">

source:media:type, src:mt
<source media="(min-width: )" srcset="" type="image/">

source:media:sizes, src:mz
<source media="(min-width: )" srcset="" sizes="">

source:sizes:type, src:zt
<source sizes="" srcset="" type="image/">

iframe
<iframe src="" frameborder="0"></iframe>

embed
<embed src="" type="">

object
<object data="" type=""></object>

param
<param name="" value="">

map
<map name=""></map>

area
<area shape="" coords="" href="" alt="">

area:d
<area shape="default" coords="" href="" alt="">

area:c
<area shape="circle" coords="" href="" alt="">

area:r
<area shape="rect" coords="" href="" alt="">

area:p
<area shape="poly" coords="" href="" alt="">

form
<form action=""></form>

form:get
<form action="" method="get"></form>

form:post
<form action="" method="post"></form>
 
 label
<label for=""></label>

input
<input type="text">

inp
<input type="text" name="" id="">

input:hidden, input:h
<input type="hidden" name="">

input:text, input:t
<input type="text" name="" id="">

input:search
<input type="search" name="" id="">

input:email
<input type="email" name="" id="">

input:url
<input type="url" name="" id="">

input:password, input:p
<input type="password" name="" id="">

input:datetime
<input type="datetime" name="" id="">

input:date
<input type="date" name="" id="">

input:datetime-local
<input type="datetime-local" name="" id="">

input:month
<input type="month" name="" id="">

input:week
<input type="week" name="" id="">

input:time
<input type="time" name="" id="">

input:tel
<input type="tel" name="" id="">

input:number
<input type="number" name="" id="">

input:color
<input type="color" name="" id="">

input:checkbox, input:c
<input type="checkbox" name="" id="">

input:radio, input:r
<input type="radio" name="" id="">

input:range
<input type="range" name="" id="">

input:file, input:f
<input type="file" name="" id="">

input:submit, input:s
<input type="submit" value="">

input:image, input:i
<input type="image" src="" alt="">

input:button, input:b
<input type="button" value="">

isindex
<isindex>

input:reset
<input type="reset" value="">

select
<select name="" id=""></select>

select:disabled, select:d
<select name="" id="" disabled="disabled"></select>

opt
<option value=""></option>

textarea
<textarea name="" id="" cols="30" rows="10"></textarea>

marquee
<marquee behavior="" direction=""></marquee>

menu:context, menu:c
<menu type="context"></menu>

menu:toolbar, menu:t
<menu type="toolbar"></menu>

video
<video src=""></video>

audio
<audio src=""></audio>

html:xml
<html xmlns="http://www.w3.org/1999/xhtml"></html>

keygen
<keygen>

command
<command>

button:submit, button:s, btn:s
<button type="submit"></button>

button:reset, button:r, btn:r
<button type="reset"></button>

button:disabled, fieldsetLd, fset:d, fst:d
<fieldset disabled="disabled"></fieldset>

bq
<blockquote></blockquote>

fig
<figure></figure>

figc
<figcaption></figcaption>

pic
<picture></picture>

ifr
<iframe src="" frameborder="0"></iframe>

emb
<embed src="" type="">

obj
<object data="" type=""></object>

cap
<caption></caption>

colg
<colgroup></colgroup>

fst, fset
<fieldset></fieldset>

btn
<button></button>

optg
<optgroup></optgroup>

tarea
<textarea name="" id="" cols="30" rows="10"></textarea>

leg
<legend></legend>

sect
<section></section>

art
<article></article>

hdr
<header></header>

ftr
<footer></footer>

adr
<address></address>

dlg
<dialog></dialog>

str
<strong></strong>

prog
<progress></progress>

mn
<main></main>

tem
<template></template>

datag
<datagrid></datagrid>

datal
<datalist></datalist>

kg
<keygen>

out
<output></output>

det
<details></details>

cmd
<command>

doc
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

ri:dpr, ri:d
        <img src="" alt="" srcset="">

ri:viewport, ri:v
<img src="" alt="" sizes="" srcset="">

ri:art, ri:a
<picture>
    <source media="(min-width: )" srcset="">
    <img src="" alt="">
</picture>

ri:type, ri:t
<picture>
    <source srcset="" type="image/">
    <img src="" alt="">
</picture>

html:5
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

ol>li
<ol>
    <li></li>
</ol>

ul>li
<ul>
    <li></li>
</ul>

dl>dt+dd
<dl>
    <dt></dt>
    <dd></dd>
</dl>

map>area
  <map name="">
      <area shape="" coords="" href="" alt="">
  </map>

table>tr>td
<table>
    <tr>
        <td></td>
    </tr>
</table>

colgroup>col
<colgroup>
    <col>
</colgroup>

tr>td
<tr>
    <td></td>
</tr>

select>option
<select name="" id="">
    <option value=""></option>
</select>

optgroup>option
  <optgroup>
            <option value=""></option>
        </optgroup>

picture>source:srcset+img
<picture>
    <source srcset="">
    <img src="" alt="">
</picture>

!!!
 <!DOCTYPE html>

 c
       <!--  -->

cc:ie
<!--[if IE]><![endif]-->

cc:noie
<!--[if !IE]><!--><!--<![endif]-->
```
### CSS
```css
pos                     position: relative;

pos:s                   position: static;

pos:a                   position: absolute;

pos:r                   position: relative;

pos:f                   position: fixed;

t                       top: ;

t:a                     top: auto;

r                       right: ;

r:a                     right: auto;

b                       bottom: ;

b:a                     bottom: auto;

l:a                     left: auto;

z                       z-index: ;

z:a                     z-index: auto;

fl                      float: left;

fl:n                    float: none;

fl:l                    float: left;

fl:r                    float: right;

cl                      clear: both;

cl:n                    clear: none;

cl:l                    clear: left;

cl:r                    clear: right;

cl:b                    clear: both;

d                       display: block;

d:n                     display: none;

d:b                     display: block;

d:f                     display: flex;

d:if                    display: inline-flex;

d:i                     display: inline;

d:ib                    display: inline-block;

d:li                    display: list-item;

d:ri                    display: run-in;

d:cp                    display: compact;

d:tb                    display: table;

d:itb                   display: inline-table;

d:tbcp                  display: table-caption;

d:tbcl                  display: table-cell;

d:tbclg                 display: table-column-group;

d:tbhg                  display: table-header-group;

d:tbfg                  display: table-footer-group;

d:tbr                   display: table-row;

d:tbrg                  display: table-row-group;

d:tbc                   display: table-cell;

d:rb                    display: ruby;

d:rbt                   display: ruby-text;

d:rbtg                  display: ruby-text-group;

v                       visibility: hidden;

v:v                     visibility: visible;

v:h                     visibility: hidden;

v:c                     visibility: collapse;

ov                      overflow: hidden;

ov:v                    overflow: visible;

ov:h                    overflow: hidden;

ov:s                    overflow: scroll;

ov:a                    overflow: auto;

ovx                     overflow-x: hidden;

ovx:v                   overflow-x: visible;

ovx:h                   overflow-x: hidden;

ovx:s                   overflow-x: scroll;

ovx:a                   overflow-x: auto;

ovy                     overflow-y: hidden;

ovy:v                   overflow-y: visible;

ovy:h                   overflow-y: hidden;

ovy:s                   overflow-y: scroll;

ovy:a                   overflow-y: auto;

ovs                     overflow-style: scrollbar;

ovs:a                   overflow-style: auto;

ovs:s                   overflow-style: scrollbar;

ovs:p                   overflow-style: panner;

ovs:m                   overflow-style: move;

ovs:mq                  overflow-style: marquee;

zoo, zm                 zoom: 1;

cp                      clip: auto;

cp:a                    clip: auto;

cp:r                    clip: rect(top right bottom left);

rsz                     resize: none;

rsz:n                   resize: none;

rsz:b                   resize: both;

rsz:h                   resize: horizontal;

rsz:v                   resize: vertical;

cur                     cursor: pointer;

cur:a                   cursor: auto;

cur:d                   cursor: default;

cur:c                   cursor: crosshair;

cur:ha                  cursor: hand;

cur:he                  cursor: help;

cur:m                   cursor: move;

cur:p                   cursor: pointer;

cur:t                   cursor: text;
```

### Margin & Padding
``` css

m                       margin: ;

m:a                     margin: auto;

mt                      margin-top: ;

mt:a                    margin-top: auto;

mr                      margin-right: ;

mr:a                    margin-right: auto;

mb                      margin-bottom: ;

mb:a                    margin-bottom: auto;

ml                      margin-left: ;

ml:a                    margin-left: auto;

p                       padding: ;

pt                      padding-top: ;

pr                      padding-right: ;

pb                      padding-bottom: ;

pl                      padding-left: ;
```

### Box Sizing

``` css
bxz                    box-sizing: border-box;

bxz:cb                 box-sizing: content-box;

bxz:bb                 box-sizing: border-box;

bxsh                   box-shadow: inset hoff voff blur #000;

bxsh:r                 box-shadow: r;

bxsh:ra                box-shadow: ra;

bxsh:n                 box-shadow: none;

w                      width: ;

w:a                    width: auto;

h                      height: ;

h:a                    height: auto;

maw                    max-width: ;

maw:n                  max-width: none;

mah                    max-height: ;

mah:n                  max-height: none;

miw                    min-width: ;

mih                    min-height: ;

```
### Font
```
f                     font: 1em sans-serif;

f+                    font: 1em Arial,sans-serif;

fw                    font-weight: normal;

fw:n                  font-weight: normal;

fw:b                  font-weight: bold;

fw:br                 font-weight: bolder;

fw:lr                 font-weight: lighter;

fs                    font-style: italic;

fs:n                  font-style: normal;

fs:i                  font-style: italic;

fs:o                  font-style: oblique;

fv                    font-variant: normal;

fv:n                  font-variant: normal;

fv:sc                 font-variant: small-caps;

fz                    font-size: ;

fza                   font-size-adjust: ;

fza:n                 font-size-adjust: none;

ff                    font-family: serif;

ff:s                  font-family: serif;

ff:ss                 font-family: sans-serif;

ff:c                  font-family: cursive;

ff:f                  font-family: fantasy;

ff:m                  font-family: monospace;

ff:a                  font-family: auto;

ff:t                  font-family: t;

ff:v                  font-family: v;

fef                   font-effect: none;

fef:n                 font-effect: none;

fef:eg                font-effect: engrave;

fef:eb                font-effect: emboss;

fef:o                 font-effect: outline;

fem                   font-emphasize: ;

femp                  font-emphasize-position: before;

femp:b                font-emphasize-position: before;

femp:a                font-emphasize-position: after;

fems                  font-emphasize-style: none;

fems:n                font-emphasize-style: none;

fems:ac               font-emphasize-style: accent;

fems:dt               font-emphasize-style: dot;

fems:c                font-emphasize-style: circle;

fems:ds               font-emphasize-style: disc;

fsm                   font-smoothing: antialiased;

fsm:a                 font-smoothing: antialiased;

fsm:n                 font-smoothing: none;

fsm:aw                font-smoothing: aw;

fst                   font-stretch: normal;

fst:uc                font-stretch: ultra-condensed;

fst:ec                font-stretch: extra-condensed;

fst:c                 font-stretch: condensed;

fst:sc                font-stretch: semi-condensed;

fst:se                font-stretch: semi-expanded;

fst:e                 font-stretch: expanded;

fst:ee                font-stretch: expanded;

fst:ue                font-stretch: ultra-expanded;

```

### Text
```css
va                    vertical-align: top;

va:sup                vertical-align: super;

va:t                  vertical-align: top;

va:tt                 vertical-align: text-top;

va:m                  vertical-align: middle;

va:bl                 vertical-align: baseline;

va:b                  vertical-align: bottom;

va:tb                 vertical-align: text-bottom;

va:sub                vertical-align: sub;

ta                    text-align: left;

ta:l                  text-align: left;

ta:c                  text-align: center;

ta:r                  text-align: right;

ta:j                  text-align: justify;

ta-lst                text-align-last: auto;

tal:a                 text-align-last: auto;

tal:l                 text-align-last: left;

tal:c                 text-align-last: center;

tal:r                 text-align-last: right;

td                    text-decoration: none;

td:n                  text-decoration: none;

td:u                  text-decoration: underline;

td:o                  text-decoration: overline;

td:l                  text-decoration: line-through;

te                    text-emphasis: none;

te:n                  text-emphasis: none;

te:ac                 text-emphasis: accent;

te:dt                 text-emphasis: dot;

te:c                  text-emphasis: circle;

te:ds                 text-emphasis: disc;

te:b                  text-emphasis: before;

te:a                  text-emphasis: after;

th                    text-height: auto;

th:a                  text-height: auto;

th:f                  text-height: font-size;

th:t                  text-height: text-size;

th:m                  text-height: max-size;

ti                    text-indent: ;

ti:-

tj                    text-justify: ;

tj:a                  text-justify: auto;

tj:iw                 text-justify: inter-word;

tj:ii                 text-justify: inter-ideograph;

tj:ic                 text-justify: inter-cluster;

tj:d                  text-justify: distribute;

tj:k                  text-justify: kashida;

tj:t                  text-justify: tibetan;

to

to+

to:n                  text-outline: none;

tr                    text-replace: ;

tr:n                  text-replace: none;

tt                    text-transform: uppercase;

tt:n                  text-transform: none;

tt:c                  text-transform: capitalize;

tt:u                  text-transform: uppercase;

tt:l                  text-transform: lowercase;

tw                    text-wrap: none;

tw:n                  text-wrap: none;

tw:no                 text-wrap: none;

tw:u                  text-wrap: unrestricted;

tw:s                  text-wrap: suppress;

tsh                   text-shadow: hoff voff blur #000;

tsh:r                 text-shadow: r;

tsh:ra                text-shadow: ra;

tsh+

tsh:n                 text-shadow: none;

lh                    line-height: ;

lts                   letter-spacing: normal;

lts-n                 letter-spacing: ;

whs                   white-space: nowrap;

whs:n                 white-space: normal;

whs:p                 white-space: pre;

whs:nw                white-space: nowrap;

whs:pw                white-space: pre-wrap;

whs:pl                white-space: pre-line;

whsc                  white-space-collapse: normal;

whsc:n                white-space-collapse: normal;

whsc:k                white-space-collapse: keep-all;

whsc:l                white-space-collapse: loose;

whsc:bs               white-space-collapse: break-strict;

whsc:ba               white-space-collapse: break-all;

wob                   word-break: normal;

wob:n                 word-break: normal;

wob:k                 word-break: keep-all;

wob:ba                word-break: break-all;

wos                   word-spacing: ;

wow                   word-wrap: ;

wow:nm                word-wrap: normal;

wow:n                 word-wrap: none;

wow:u                 word-wrap: unrestricted;

wow:s                 word-wrap: suppress;

wow:b                 word-wrap: break-word;

```

### Background

```css

```

### Color

```css
c                     color: #000;

c:r                   color: r;

c:ra                  color: ra;

op                    opacity: ;

```

### Generated Content

```css

```

### Outline

```css

```

### Tables

```css
tbl                   table-layout: fixed;

tbl:a                 table-layout: auto;

tbl:f                 table-layout: fixed;

cps                   caption-side: top;

cps:t                 caption-side: top;

cps:b                 caption-side: bottom;

ec                    empty-cells: show;

ec:s                  empty-cells: show;

ec:h                  empty-cells: hide;

```

### Border

```css

```

### Lists

```css
lis                   list-style: ;

lis:n                 list-style: none;

lisp                  list-style-position: inside;

lisp:i                list-style-position: inside;

lisp:o                list-style-position: outside;

list                  list-style: ;

list:n                list-style-type: none;

list:d                list-style-type: disc;

list:c                list-style-type: circle;

list:s                list-style-type: square;

list:dc               list-style-type: disc;

list:dclz             list-style-type: decimal-leading-zero;

list:lr               list-style-type: lower-roman;

list:ur               list-style-type: upper-roman;

lisi                  list-style-image: inherit;

lisi:n                list-style-image: none;

```

### Print

```css
pgbb                page-break-before: auto;

pgbb:au             page-break-before: auto;            

pgbb:al             page-break-before: always;

pgbb:l              page-break-before: left;

pgbb:r              page-break-before: right;

pgbi                page-break-inside: auto;

pgbi:au             page-break-inside: auto;

pgbi:al             page-break-inside: always;

pgbi:l              page-break-inside: left;

pgbi:r              page-break-inside: right;

orp                 orphans: ;

wid                 width: ;

```

### Others

```css
!         
!important

@f
@font-face { font-family:; src:url(|); }

@f+
@font-face { font-family: 'FontName'; src: url('FileName.eot'); src: url('FileName.eot?#iefix') format('embedded-opentype'), url('FileName.woff') format('woff'), url('FileName.ttf') format('truetype'), url('FileName.svg#FontName') format('svg'); font-style: normal; font-weight: normal; }

@i, @import
@import url();

@kf
@-webkit-keyframes identifier { from { } to { } } @-o-keyframes identifier { from { } to { } } @-moz-keyframes identifier { from { } to { } } @keyframes identifier { from { } to { } }

@m, @media
@media screen { }

ac                        align-content:;

ac:c                      align-content:center;

ac:fe                     align-content:flex-end;

ac:fs                     align-content:flex-start;

ac:s                      align-content:stretch;

ac:sa                     align-content:space-around;

ac:sb                     align-content:space-between;

ai                        align-items:;
ai:b                      align-items:baseline;
ai:c                      align-items:center;
ai:fe                     align-items:flex-end;
ai:fs                     align-items:flex-start;
ai:s                      align-items:stretch;
anim                      
 animation:;
anim-
animation:name duration timing-function delay iteration-count direction fill-mode;

animdel                   animation-delay:time;
animdir                   animation-direction:normal;
animdir:a                 animation-direction:alternate;
animdir:ar          animation-direction:alternate-reverse;
animdir:n                 animation-direction:normal;
animdir:r                 animation-direction:reverse;
animdur                   animation-duration:0s;
animfm                    animation-fill-mode:both;
animfm:b                  animation-fill-mode:backwards;
animfm:bt, animfm:bh      animation-fill-mode:both;
animfm:f                  animation-fill-mode:forwards;
animic                    animation-iteration-count:1;
animic:i               animation-iteration-count:infinite;
animn                     animation-name:none;
animps                    animation-play-state:running;
animps:p                  animation-play-state:paused;
animps:r                  animation-play-state:running;
animtf                   animation-timing-function:linear;
animtf:cb           animation-timing-function:cubic-bezier(0.1, 0.7, 1.0, 0.1);
animtf:e           animation-timing-function:ease;
animtf:ei           animation-timing-function:ease-in;
animtf:eio           animation-timing-function:ease-in-out;
animtf:eo           animation-timing-function:ease-out;
animtf:l           animation-timing-function:linear;
ap           appearance:${none};
as           align-self:;
as:a           align-self:auto;
as:b           align-self:baseline;
as:c           align-self:center;
as:fe           align-self:flex-end;
as:fs           align-self:flex-start;
as:s             align-self:stretch;
bfv               backface-visibility:;
bfv:h             backface-visibility:hidden;
bfv:v             backface-visibility:visible;
bg:ie
filter:progid:DXImageTransform.Microsoft.AlphaImageLoader(src='x.png',sizingMethod='crop');
cm
/* ${child} */
colm                   columns:;
colmc                   column-count:;
colmf                   column-fill:;
colmg                   column-gap:;
colmr                   column-rule:;
colmrc                   column-rule-color:;
colmrs                   column-rule-style:;
colmrw                   column-rule-width:;
colms                   column-span:;
colmw                   column-width:;
d:ib+  display: inline-block; *display: inline; *zoom: 1;
fx
flex:;
fxb
flex-basis:;
fxd
flex-direction:;
fxd:c
flex-direction:column;
fxd:cr
flex-direction:column-reverse;
fxd:r
flex-direction:row;
fxd:rr
flex-direction:row-reverse;
fxf
flex-flow:;
fxg
flex-grow:;
fxsh
flex-shrink:;
fxw
flex-wrap: ;
fxw:n
flex-wrap:nowrap;
fxw:w
flex-wrap:wrap;
fxw:wr
flex-wrap:wrap-reverse;
jc
justify-content:;
jc:c
justify-content:center;
jc:fe
justify-content:flex-end;
jc:fs
justify-content:flex-start;
jc:sa
justify-content:space-around;
jc:sb
justify-content:space-between;
mar
max-resolution:res;
mir
min-resolution:res;
op+
opacity: ; filter: alpha(opacity=);
op:ie
filter:progid:DXImageTransform.Microsoft.Alpha(Opacity=100);
op:ms
-ms-filter:'progid:DXImageTransform.Microsoft.Alpha(Opacity=100)';
ord
order:;
ori
orientation:;
ori:l
orientation:landscape;
ori:p
orientation:portrait;
tov
text-overflow:${ellipsis};
tov:c
text-overflow:clip;
tov:e
text-overflow:ellipsis;
trf
transform:;
trf:r
transform: rotate(angle);
trf:rx
transform: rotateX(angle);
trf:ry
transform: rotateY(angle);
trf:rz
transform: rotateZ(angle);
trf:sc
transform: scale(x, y);
trf:sc3
transform: scale3d(x, y, z);
trf:scx
transform: scaleX(x);
trf:scy
transform: scaleY(y);
trf:scz
transform: scaleZ(z);
trf:skx
transform: skewX(angle);
trf:sky
transform: skewY(angle);
trf:t
transform: translate(x, y);
trf:t3
transform: translate3d(tx, ty, tz);
trf:tx
transform: translateX(x);
trf:ty
transform: translateY(y);
trf:tz
transform: translateZ(z);
trfo
transform-origin:;
trfs
transform-style:preserve-3d;
trs
transition:prop time;
trsde
transition-delay:time;
trsdu
transition-duration:time;
trsp
transition-property:prop;
trstf
transition-timing-function:tfunc;
us
user-select:${none};
wfsm
-webkit-font-smoothing:${antialiased};
wfsm:a
-webkit-font-smoothing:antialiased;
wfsm:n
-webkit-font-smoothing:none;
wfsm:s, wfsm:sa                    -webkit-font-smoothing:subpixel-antialiased;
wm                    writing-mode:lr-tb;
wm:btl                    writing-mode:bt-lr;
wm:btr                    writing-mode:bt-rl;
wm:lrb                    writing-mode:lr-bt;
wm:lrt                    writing-mode:lr-tb;
wm:rlb                    writing-mode:rl-bt;
wm:rlt                    writing-mode:rl-tb;
wm:tbl                    writing-mode:tb-lr;
wm:tbr                    writing-mode:tb-rl;
```

### XSL

```xsl
tmatch, tm
<xsl:template match="" mode=""></xsl:template>

tname, tn
<xsl:template name=""></xsl:template>

call
<xsl:call-template name="" />

ap
<xsl:apply-templates select="" mode="" />

api
<xsl:apply-imports />

imp
<xsl:import href="" />

inc
<xsl:include href="" />

ch
<xsl:choose></xsl:choose>

xsl:when, wh
<xsl:when test=""></xsl:when>

ot
<xsl:otherwise></xsl:otherwise>

if
<xsl:if test=""></xsl:if>

par
<xsl:param name=""></xsl:param>

pare
<xsl:param name="" select="" />

var
<xsl:variable name=""></xsl:variable>

vare
<xsl:variable name="" select="" />

wp
<xsl:with-param name="" select="" />

key
<xsl:key name="" match="" use="" />

elem
<xsl:element name=""></xsl:element>

attr
<xsl:attribute name=""></xsl:attribute>

attrs
<xsl:attribute-set name=""></xsl:attribute-set>

cp
<xsl:copy select="" />

co
<xsl:copy-of select="" />

val
<xsl:value-of select="" />

each, for
<xsl:for-each select=""></xsl:for-each>

tex
<xsl:text></xsl:text>

com
<xsl:comment></xsl:comment>

msg
<xsl:message terminate="no"></xsl:message>

fall
<xsl:fallback></xsl:fallback>

num
<xsl:number value="" />

nam
<namespace-alias stylesheet-prefix="" result-prefix="" />

pres
<xsl:preserve-space elements="" />

strip
<xsl:strip-space elements="" />

proc
<xsl:processing-instruction name=""></xsl:processing-instruction>

sort
<xsl:sort select="" order="" />

choose+
Alias of xsl:choose>xsl:when+xsl:otherwise

<xsl:choose> <xsl:when test=""></xsl:when> <xsl:otherwise></xsl:otherwise> </xsl:choose>

xsl
Alias of !!!+xsl:stylesheet[version=1.0 xmlns:xsl=http://www.w3.org/1999/XSL/Transform]>{ |}

<?xml version="1.0" encoding="UTF-8"?> <xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform"></xsl:stylesheet>

!!!
<?xml version="1.0" encoding="UTF-8"?>

```
