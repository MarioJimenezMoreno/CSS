# SPEEDRUN

## Ejercicio Intro
\<ul>  
➡      \<li>\</li>  
        \<li>\</li>  
        \<li>\</li>  
    \</ul>

Respuesta: li:first-child

## Ejercicio 1
\<div>  
➡ \<p>\</p>  
  \<p class="foo">\</p>  
➡  \<p>\</p>  
➡  \<p>\</p>  
\</div>

Respuesta: p:not(.foo)

## Ejercicio 2
\<ul>  
  \<li>\</li>  
  \<li>\</li>  
➡ \<li>\</li>  
  \<li>\</li>  
➡  \<li>\</li>  
  \<li>\</li>  
➡  \<li>\</li>  
\</ul>

Respuesta: li:nth-child(2n+3)

## Ejercicio 3
\<div>  
➡  \<span>\</span>  
➡  \<p>  
    \<a>\</a>  
    \<span>\</span>  
  \</p>  
\</div>

Respuesta 1: div> span, p   
Respuesta 2: div> *

## Ejercicio 4

Respuesta: span[data-item]

## Ejercicio 5

\<div>  
    \<span>\</span>  
    \<code>\</code>  
    \<span>\</span>  
    \<p>\</p>  
 ➡ \<span>\</span>  
 ➡ \<span>\</span>  
    \<p>\</p>  
    \<code>\</code>  
 ➡ \<span>\</span>  
    \<p>\</p>  
\</div>  

Respuesta: span:nth-child(1n+4)
Respuesta 2: p ~ span

## Ejercicio 6

\<form>  
➡  \<input />  
    \<input disabled />  
➡  \<input />  
➡  \<input />  
    \<button disabled>\</button>  
➡  \<button>\</button>  
\</form>

Respuesta 1: input:enabled,button:enabled  
Respuesta 2: :enabled

## Ejercicio 7

\<ol>  
➡  \<li class="me" id="one">\</li>  
➡  \<li class="you" id="two">\</li>  
    \<li class="me" id="three">\</li>  
    \<li class="you" id="four">\</li>  
➡  \<li class="me" id="five">\</li>  
➡  \<li class="you" id="six">\</li>  
    \<li class="me" id="seven">\</li>  
    \<li class="you" id="eight">\</li>  
➡  \<li class="me" id="nine">\</li>  
    \<li class="you" id="ten">\</li>  
\</ol>  

Respuesta 1:li.me:nth-child(4n+1),li.you:nth-last-child(4n+5)  
Respuesta 2: #one, #two, #five, #six, #nine

## Ejercicio 8

\<div>  
  \<span>\</span>  
  \<p>  
    \<a>\</a>  
➡  \<span>\</span>  
  \</p>  
  \<p>  
    \<span>\</span>  
    \<a>\</a>  
➡  \<span>\</span>  
    \<span>\</span>  
  \</p>  
    \<a>\</a>  
➡  \<span>\</span>  
\</div>  

Respuesta: a + span  

## Ejercicio 9

\<div id="foo">  
➡  \<div class="foo">\</div>  
    \<div>\</div>  
    \<div>  
      \<div class="foo">\</div>  
      \<div>\</div>  
    \</div>  
➡  \<div class="foo">\</div>  
\</div>  

Respuesta 1: div#foo > .foo
Respuesta 2: #foo > .foo

## Ejercicio 10

\<div>  
  \<div>  
    \<span>\</span>  
➡  \<code>\</code>  
  \</div>  
  \<div>  
    \<code>\</code>  
    \<span>\</span>  
➡  \<code>\</code>  
  \</div>  
  \<div>  
    \<span>\</span>  
    \<code class="foo">\</code>  
  \</div>  
  \<span>\</span>  
  \<code>\</code>  
\</div>  

Respuesta 1: div > div:nth-child(-n+2)  > span + code  
Respuesta 2: div div span + code:not(.foo)