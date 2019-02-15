The first steps:
1) Create email account at https://temp-mail.org/
2) Create an account at https://avocode.com/
 2.1) Avocode in 10 minutes: https://www.youtube.com/watch?v=pAfMkjKY004 
 2.2) Russian free equivalent: https://www.markupeasy.ru 
                   + tutorial: https://www.youtube.com/watch?v=CQUjRKP2op8
                   + VK group: https://vk.com/markupeasy
3) Download Sublime Text 3
 3.1) Useful plugins for  ST3: https://proglib.io/p/15-sublime-text-plugins/
4) Download SRware [look like safari | webkit engine] https://www.srware.net/en/software_srware_iron_download.php
Get down to work

Teacher:
Igor Kubikov

Useful links:
https://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048
https://fontawesome.com
       <i class="fas fa-shopping-cart"></i>
       <i class="fas fa-caret-down"></i>
       <i class="fas fa-search"></i>
       http://fontawesome.ru/examples/
http://www.html-color-names.com/color-chart.php
https://caniuse.com/
https://validator.w3.org/#validate_by_input
https://www.liveinternet.ru/stat/ru/browsers.html?date=2018-04-01;period=month
https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi
https://flexboxfroggy.com/#ru
https://code.visualstudio.com/
https://marketplace.visualstudio.com/VSCode  https://yadi.sk/i/yZkNB89f3ZXpqY

<!-- Regular Expression Language <lang="ru"> -->
https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference
http://www.pcre.ru/docs/perl/text/intro
    i - не различать строчные и заглавные буквы;
    m - считать строку многострочной;
    s - однострочная строка;
    x - расширенный синтаксис ( использование пробелов и комментариев).

Обычно все эти опции обозначают как '/x'. Их можно использовать даже внутри шаблонов использую новую конструкцию (?...).

В шаблонах используются следующие метасимволы (символы обозначающие группы других символов):

    \ - считать следующий метасимвол как обычный символ;
    ^ - начало строки;
    . - один произвольный символ. Кроме '\n' - конец строки;
    $ - конец строки;
    | - альтернатива (или);
    () - группировка;
    [ ] - класс символов.

Метасимволы имеют модификаторы (пишутся после метасимвола):

    * - повторяется 0 или большее число раз;
    + - повторяется 1 или большее число раз;
    ? - 1 или 0 раз;
    {n} - точно n раз;
    {n,} - по меньшей мере раз;
    {n,m} - не менше n, но и не больше m.

Во все других случаях фигурные скобки считаются обычными (регулярными) символами. Таким образом '*' эквивалентна {0,} , '+' - {1,} и '?' - {0,1}. n и m не могут быть больше 65536.

По умолчанию действие метасимволов «жадно» (greedy). Совпадение распространяется столько раз сколько возможно не учитывая результат действия следуюющих метасимволов. Если вы хотите "уменьшить их аппетит" то используйте символ '?'. Это не изменяет значение метасимволов просто уменьшает распространение. Таким образом:

    *? - станет 0 и более;
    +? - 1 и более;
    ?? - 0 или 1 раз;
    {n}? - точно n раз;
    {n,}? - не меньше n раз;
    {n,m}? - больше или равно n и меньше m раз.

Шаблоны работают так же, как и двойные кавычки поэтому в них можно использовать `\` - символы (бакслэш-символы):

    \t - символ табуляции;
    \n - новая строка;
    \r - перевод каретки;
    \а - перевол формата;
    \v - вертикальная табуляция;
    \a - звонок;
    \e - escape;
    \033 - восьмеричная запись символа;
    \x1A - шестнадцатеричная;
    \c[ - control символ;
    \l - нижний регистр следующего символа;
    \u - верхний регистр следующего символа;
    \L - все символы в нижнем регистре до \E;
    \U - в верхнем регистре до \E;
    \E - ограничитель смены регистра;
    \Q - отмена действия как метасимвола.

Дополнительно в Perl добавлены следующие метасимволы:

    \w - алфавитно-цифровой или '_' символ;
    \W - не алфавитно-цифровой или '_' символ;
    \s - один пробел;
    \S - один не пробел;
    \d - одна цифра;
    \D - одна не цифра.

Обратите внимание что все это «один» символ. Для обозначения последовательности применяйте модификаторы, например:

    \w+ - слово;
    \d+ - целое число;
    [+-]?\d+ - целое со знаком;
    [+-]?\d+\.?\d* - число с точкой.

Кроме того существуют мнимые метасимволы. Обозначающие не существующие символы в месте смены значения. Такие как:

    \b - граница слова;
    \B - не граница слова;
    \A - начало строки;
    \Z - конец строки;
    \G - конец действия m//g.

Граница слова (\b) - это мнимая точка между символами \w и \W. Внутри класса символов '\b' обозначает символ backspace (стирания). Метасимволы \A и \Z - аналогичны '^' и '$' но если началостроки '^' и конец строки '$' действуют для каждой строки в многосторочной строке, то \A и \Z обозначают начало и конец всей многосторчной строки.

Если внутри шаблона применяется группировка (круглые скобки) то номер подстроки группы обозначается как '\цифра'.

Заметьте что за шаблоном в пределах выражения или блока эти группы обозначаются как '$цифра'. Кроме этого существуют дополнительные переменные:

    $+ - обозначает последнее совпадение;
    $& - все совпадение;
    $` - все до совпадения;
    $' - все после совпадения.

Пример:

$s = "Один 1 два 2 и три 3";
if ($s =~ /(\d+)\D+(\d+)/)
{
print "$1\n"; # Результат '1'
print "$2\n"; # '2'
print "$+\n"; # '2'
print "$&\n"; # '1 два 2'
print "$`\n"; # 'Один '
print "$'\n"; # ' и три 3'
}

Perl версии 5 содержит дополнительные конструкции шаблонов:

    (?#комментарий) - комментарий в теле шаблона.
    (?:шаблон) - группировка как и '( )' но без обратной ссылки.
    (?=шаблон) - "заглядывание" вперед.

Например /\w+(?=\t)/ соответствует слову, за которым идет табуляция, но символ '\t' не включается в результат.

Пример:

$s = "1+2-3*4";
if ($s =~ /(\d)(?=-)/) # Наити цифру за которой стоит '-'
{
print "$1\n"; # Результат '2'
} else {
print "ошибка поиска\n";
}

(?!шаблон) - "заглядывание" вперед по отрицанию.

Пример:

$s = "1+2-3*4";
if ($s =~ /(\d)(?!\+)/) # Наити цифру за которой не стоит '+'
{
print "$1\n"; # Результат '2'
} else {
print "ошибка поиска\n";
}

(?ismx) - "внутренние" модификаторы. Удобно применять в шаблонах, где например нужно внутри шаблона указать модификатор.

Правила регулярных выражений

    Любой символ обозначает себя самого если это не метасимвол. Если вам нужно отменить действие метасимвола то поставьте перед ним '\'.
    Строка символов обозначает строку этих символов.
    Множество возможных символов (класс) заключается в квадратные скобки '[]' это значит что в данном месте может стоять один из указанных в скобках символ. Если первый символ в скобках это '^' - значит не один из указанных символов не может стоять в данном месте выражения. Внутри класса можно употреблять символ '-' обозначающий диаппазон символов. Например a-z один из малых букв латинского алфавита, 0-9 - цифра и т.д.
    Все символы, включая специальные можно обозначать с помощью '\' как в языке С.
    Альтернативные последовательности разделяются символом '|' Заметьте, что внутри квадратных скобок это обычный символ.
    Внутри регулярного выражения можно указыват "подшаблоны", заключая их в крунлые скобки и ссылаться на них как '\номер' Первая скобка обозначается как '\1'.
    
EMMET

Сокращение
	
Расшифровка сокращения
Базовый синтаксис EMMET
Дочерний: > 	

    code
    source

    nav>ul>li
    <nav>
        <ul>
            <li></li>
        </ul>
    </nav>

Соединение: + 	

    code
    source

    div+p+bq
    <div></div>
    <p></p>
    <blockquote></blockquote>

Поместить выше (в дереве HTML): ^ 	

    code
    source

    div>p>span+em^bq
    <div>
        <p><span></span><em></em></p>
        <blockquote></blockquote>
    </div>

Группировать: () 	

    code
    source

    div>(header>ul>li)+footer>p
        <div>
        <header>
            <ul>
                <li></li>
            </ul>
        </header>
        <footer>
            <p></p>
            </footer>
    </div>

Умножение: * 	

    code
    source

    ul>li*3
    <ul>
        <li></li>
        <li></li>
        <li></li>
    </ul>

Нумерация: $ 	

    code
    source

    ul>li.item_$*3
    <ul>
        <li class="item_1"></li>
        <li class="item_2"></li>
        <li class="item_3"></li>
    </ul>

id и class 	

    code
    source

    #header+.class
    <div id="header"></div>
    <div class="class"></div>

    #hdr.cl_1.cl_2
    <div id="hdr" class="cl_1 cl_2"></div>

Атрибуты: [] 	

    code
    source

    a[title="Подсказка ссылки"]
    <a href="" title="Подсказка ссылки"></a>

    td[rowspan colspan title]
    <td rowspan="" colspan="" title=""></td>

Текст: {} 	

    code
    source

    .class{свободный текст}
    <div class="class">свободный текст</div>

    p>{Кликните }+a{сюда}+{ скорее}
    <p>Кликните <a href="">сюда</a> скорее</p>

Сокращение тегов 	

    code
    source

    .class
    <div class="class"></div>

    em>.class
    <em><span class="class"></span></em>

    ul>.class
    <ul>
        <li class="class"></li>
    </ul>

    table>.row>.col
    <table>
        <tr class="row">
            <td class="col"></td>
        </tr>
    </table>

HTML сокращения
! 	

    code
    source

    <!doctype html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>Document</title>
        </head>
        <body>

        </body>
    </html>

a 	

    code
    source

    <a href=""></a>

a:link 	

    code
    source

    <a href="http://"></a>

a:mail 	

    code
    source

    <a href="mailto:"></a>

base 	

    code
    source

    <base href="">

br 	

    code
    source

    <br>

link 	

    code
    source

    <link rel="stylesheet" href="">

link:css 	

    code
    source

    <link rel="stylesheet" href="style.css">

link:favicon 	

    code
    source

    <link rel="shortcut icon" type="image/x-icon"
    href="favicon.ico">

link:rss 	

    code
    source

    <link rel="alternate" type="application/rss+xml"
    title="RSS" href="rss.xml">

link:atom 	

    code
    source

    <link rel="alternate" type="application/atom+xml"
    title="Atom" href="atom.xml">

meta:utf 	

    code
    source

    <meta http-equiv="Content-Type"
    content="text/html;charset=UTF-8">

meta:vp 	

    code
    source

    <meta name="viewport" content="width=device-width,
    user-scalable=no, initial-scale=1.0,
    maximum-scale=1.0, minimum-scale=1.0">

meta:compat 	

    code
    source

    <meta http-equiv="X-UA-Compatible" content="IE=7">

script:src 	

    code
    source

    <script src=""></script>

img 	

    code
    source

    <img src="" alt="">

ifr 	

    code
    source

    <iframe src="" frameborder="0"></iframe>

emb 	

    code
    source

    <embed src="" type="">

obj 	

    code
    source

    <object data="" type=""></object>

map 	

    code
    source

    <map name=""></map>

map+ 	

    code
    source

    <map name="">
        <area shape="" coords="" href="" alt="">
    </map>

area 	

    code
    source

    <area shape="" coords="" href="" alt="">

form 	

    code
    source

    <form action=""></form>

form:get
form:post 	

    code
    source

    <form action="" method="get"></form>
    <form action="" method="post"></form>

label 	

    code
    source

    <label for=""></label>

input 	

    code
    source

    <input type="text">

inp 	

    code
    source

    <input type="text" name="" id="">

input:h 	

    code
    source

    <input type="hidden" name="">

input:p 	

    code
    source

    <input type="password" name="" id="">

input:c 	

    code
    source

    <input type="checkbox" name="" id="">

input:r 	

    code
    source

    <input type="radio" name="" id="">

input:f 	

    code
    source

    <input type="file" name="" id="">

input:s 	

    code
    source

    <input type="submit" value="">

input:i 	

    code
    source

    <input type="image" src="" alt="">

input:b 	

    code
    source

    <input type="button" value="">

input:reset 	

    code
    source

    <input type="reset" value="">

select 	

    code
    source

    <select name="" id=""></select>

select+ 	

    code
    source

    <select name="" id="">
        <option value=""></option>
    </select>

opt 	

    code
    source

    <option value=""></option>

tarea 	

    code
    source

    <textarea name="" id="" cols="30" rows="10">
    </textarea>

video 	

    code
    source

    <video src=""></video>

audio 	

    code
    source

    <audio src=""></audio>

bq 	

    code
    source

    <blockquote></blockquote>

fst 	

    code
    source

    <fieldset></fieldset>

btn 	

    code
    source

    <button></button>

btn:s 	

    code
    source

    <button type="submit"></button>

btn:b 	

    code
    source

    <button type="button"></button>

btn:r 	

    code
    source

    <button type="reset"></button>

sect 	

    code
    source

    <section></section>

art 	

    code
    source

    <article></article>

hdr 	

    code
    source

    <header></header>

ftr 	

    code
    source

    <footer></footer>

str 	

    code
    source

    <strong></strong>

ol+ 	

    code
    source

    <ol>
        <li></li>
    </ol>

ul+ 	

    code
    source

    <ul>
        <li></li>
    </ul>

dl+ 	

    code
    source

    <dl>
        <dt></dt>
        <dd></dd>
    </dl>

table+ 	

    code
    source

    <table>
        <tr>
            <td></td>
        </tr>
    </table>

tr+ 	

    code
    source

    <tr>
        <td></td>
    </tr>

c 	

    code
    source

    <!-- Комментарий -->

cc:ie6 	

    code
    source

    <!--[if lte IE 6]>

    <![endif]-->

cc:ie 	

    code
    source

    <!--[if IE]>

    <![endif]-->

cc:noie 	

    code
    source

    <!--[if !IE]><!-->

    <!--<![endif]-->

Любой тег 	

    code
    source

    div
    <div></div>

    span
    <span></span>

    Любой другой тег
    <tagname></tagname>

CSS сокращения
pos 	

    code
    source

    position: relative;

posa 	

    code
    source

    position: absolute;

posr 	

    code
    source

    position: relative;

posf 	

    code
    source

    position: fixed;

t 	

    code
    source

    top: ;

t:a 	

    code
    source

    top: auto;

r 	

    code
    source

    right: ;

r:a 	

    code
    source

    right: auto;

b 	

    code
    source

    bottom: ;

b:a 	

    code
    source

    bottom: auto;

l 	

    code
    source

    left: ;

l:a 	

    code
    source

    left: auto;

z 	

    code
    source

    z-index: ;

za 	

    code
    source

    z-index: auto;

fl 	

    code
    source

    float: left;

fln 	

    code
    source

    float: none;

fr 	

    code
    source

    float: right;

cl 	

    code
    source

    clear: both;

d 	

    code
    source

    display: block;

dn 	

    code
    source

    display: none;

di 	

    code
    source

    display: inline;

dib 	

    code
    source

    display: inline-block;

dt 	

    code
    source

    display: table;

dtc 	

    code
    source

    display: table-cell;

dtr 	

    code
    source

    display: table-row;

v 	

    code
    source

    visibility: hidden;

vv 	

    code
    source

    visibility: visible;

oh 	

    code
    source

    overflow: hidden;

ovv 	

    code
    source

    overflow: visible;

os 	

    code
    source

    overflow: scroll;

oa 	

    code
    source

    overflow: auto;

zm 	

    code
    source

    zoom: 1;

cu 	

    code
    source

    cursor: ;

cup 	

    code
    source

    cursor: pointer;

cud 	

    code
    source

    cursor: default;

cuh 	

    code
    source

    cursor: hand;

cuhe 	

    code
    source

    cursor: help;

cum 	

    code
    source

    cursor: move;

cut 	

    code
    source

    cursor: text;

m 	

    code
    source

    margin: ;

m:a 	

    code
    source

    margin: auto;

mt 	

    code
    source

    margin-top: ;

mta 	

    code
    source

    margin-top: auto;

mr 	

    code
    source

    margin-right: ;

mra 	

    code
    source

    margin-right: auto;

mb 	

    code
    source

    margin-bottom: ;

mba 	

    code
    source

    margin-bottom: auto;

ml 	

    code
    source

    margin-left: ;

mla 	

    code
    source

    margin-left: auto;

p 	

    code
    source

    padding: ;

pt 	

    code
    source

    padding-top: ;

pr 	

    code
    source

    padding-right: ;

pb 	

    code
    source

    padding-bottom: ;

pl 	

    code
    source

    padding-left: ;

bsh 	

    code
    source

    -webkit-box-shadow: inset hoff voff blur color;
    -moz-box-shadow: inset hoff voff blur color;
    box-shadow: inset hoff voff blur color;

bshn 	

    code
    source

    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;

w 	

    code
    source

    width: ;

wa 	

    code
    source

    width: auto;

h 	

    code
    source

    height: ;

ha 	

    code
    source

    height: auto;

maw 	

    code
    source

    max-width: ;

mah 	

    code
    source

    max-height: ;

mw 	

    code
    source

    min-width: ;

mh 	

    code
    source

    min-height: ;

f 	

    code
    source

    font: ;

f+ 	

    code
    source

    font: 1em Arial,sans-serif;

fw 	

    code
    source

    font-weight: ;

fwn 	

    code
    source

    font-weight: normal;

fwb 	

    code
    source

    font-weight: bold;

fs 	

    code
    source

    font-style: italic;

fsn 	

    code
    source

    font-style: normal;

fsi 	

    code
    source

    font-style: italic;

fz 	

    code
    source

    font-size: ;

ff 	

    code
    source

    font-family: ;

ffs 	

    code
    source

    font-family: serif;

ffss 	

    code
    source

    font-family: sans-serif;

ffm 	

    code
    source

    font-family: monospace;

ffa 	

    code
    source

    font-family: Arial, "Helvetica Neue", Helvetica,
    sans-serif;

va 	

    code
    source

    vertical-align: top;

vm 	

    code
    source

    vertical-align: middle;

vabl 	

    code
    source

    vertical-align: baseline;

vb 	

    code
    source

    vertical-align: bottom;

vs 	

    code
    source

    vertical-align: sub;

ta 	

    code
    source

    text-align: left;

tac 	

    code
    source

    text-align: center;

tar 	

    code
    source

    text-align: right;

taj 	

    code
    source

    text-align: justify;

td 	

    code
    source

    text-decoration: none;

tdu 	

    code
    source

    text-decoration: underline;

tdo 	

    code
    source

    text-decoration: overline;

tdl 	

    code
    source

    text-decoration: line-through;

tt 	

    code
    source

    text-transform: uppercase;

ttn 	

    code
    source

    text-transform: none;

ttl 	

    code
    source

    text-transform: lowercase;

ts 	

    code
    source

    text-shadow: hoff voff blur #000;

tra 	

    code
    source

    text-shadow: h v blur rgba(0, 0, 0, .5);

ts+ 	

    code
    source

    text-shadow: 0 0 0 #000;

tsn 	

    code
    source

    text-shadow: none;

lh 	

    code
    source

    line-height: ;

lts 	

    code
    source

    letter-spacing: ;

ws 	

    code
    source

    white-space: ;

wsn 	

    code
    source

    white-space: normal;

wsnw 	

    code
    source

    white-space: nowrap;

bg 	

    code
    source

    background: #000;

bg+ 	

    code
    source

    background: #fff url() 0 0 no-repeat;

bn 	

    code
    source

    background: none;

bgc 	

    code
    source

    background-color: #fff;

bgt 	

    code
    source

    background-color: transparent;

bgi 	

    code
    source

    background-image: url();

bgin 	

    code
    source

    background-image: none;

bgr 	

    code
    source

    background-repeat: ;

bgrn 	

    code
    source

    background-repeat: no-repeat;

bgrx 	

    code
    source

    background-repeat: repeat-x;

bgry 	

    code
    source

    background-repeat: repeat-y;

bga 	

    code
    source

    background-attachment: ;

baf 	

    code
    source

    background-attachment: fixed;

bas 	

    code
    source

    background-attachment: scroll;

bgp 	

    code
    source

    background-position: 0 0;

bgs 	

    code
    source

    -webkit-background-size: ;
    background-size: ;

bsa 	

    code
    source

    -webkit-background-size: auto;
    background-size: auto;

c 	

    code
    source

    color: #000;

cra 	

    code
    source

    color: rgba(0, 0, 0, .5);

op 	

    code
    source

    opacity: ;

ct 	

    code
    source

    content: '';

q 	

    code
    source

    quotes: ;

ol 	

    code
    source

    outline: ;

on 	

    code
    source

    outline: none;

tbl 	

    code
    source

    table-layout: ;

cs 	

    code
    source

    caption-side: ;

ec 	

    code
    source

    empty-cells: ;

bd 	

    code
    source

    border: ;

bd+ 	

    code
    source

    border: 1px solid #000;

bdn 	

    code
    source

    border: none;

bdc 	

    code
    source

    border-color: #000;

bdi 	

    code
    source

    -webkit-border-image: url();
    -moz-border-image: url();
    -o-border-image: url();
    border-image: url();

bdin 	

    code
    source

    -webkit-border-image: none;
    -moz-border-image: none;
    -o-border-image: none;
    border-image: none;

bf 	

    code
    source

    -webkit-border-fit: repeat;
    border-fit: repeat;

bdle 	

    code
    source

    border-length: ;

bsp 	

    code
    source

    border-spacing: ;

bds 	

    code
    source

    border-style: ;

bw 	

    code
    source

    border-width: ;

bt 	

    code
    source

    border-top: ;

bt+ 	

    code
    source

    border-top: 1px solid #000;

bdtn 	

    code
    source

    border-top: none;

br 	

    code
    source

    border-right: ;

br+ 	

    code
    source

    border-right: 1px solid #000;

bdrn 	

    code
    source

    border-right: none;

bb 	

    code
    source

    border-bottom: ;

bb+ 	

    code
    source

    border-bottom: 1px solid #000;

bdbn 	

    code
    source

    border-bottom: none;

bl 	

    code
    source

    border-left: ;

bl+ 	

    code
    source

    border-left: 1px solid #000;

bdln 	

    code
    source

    border-left: none;

bdrs 	

    code
    source

    -webkit-border-radius: ;
    -moz-border-radius: ;
    border-radius: ;

btrr 	

    code
    source

    border-top-right-radius: ;

bdtrs 	

    code
    source

    border-top-left-radius: ;

bbrr 	

    code
    source

    border-bottom-right-radius: ;

bblr 	

    code
    source

    border-bottom-left-radius: ;

lis 	

    code
    source

    list-style: ;

lisn 	

    code
    source

    list-style: none;

lst 	

    code
    source

    list-style-type: ;

lstn 	

    code
    source

    list-style-type: none;

lstd 	

    code
    source

    list-style-type: disc;

lstc 	

    code
    source

    list-style-type: circle;

lsts 	

    code
    source

    list-style-type: square;

lstdc 	

    code
    source

    list-style-type: decimal;

lsi 	

    code
    source

    list-style-image: ;

lsin 	

    code
    source

    list-style-image: none;

! 	

    code
    source

    !important

@f 	

    code
    source

    @font-face {
    font-family:;
    src:url();
    }

@f+ 	

    code
    source

    @font-face {
        font-family: 'FontName';
        src: url('FileName.eot');
        src: url('FileName.eot?#iefix')
        format('embedded-opentype'),
            url('FileName.woff') format('woff'),
            url('FileName.ttf') format('truetype'),
            url('FileName.svg#FontName') format('svg');
        font-style: normal;
        font-weight: normal;
    }

@i 	

    code
    source

    @import url();

@m 	

    code
    source

    @media screen {

    }

anim 	

    code
    source

    -webkit-animation: ;
    -o-animation: ;
    animation: ;

ap 	

    code
    source

    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;

bgie 	

    code
    source

    filter:progid:DXImageTransform
    .Microsoft.AlphaImageLoader
    (src='x.png',sizingMethod='crop');

cm 	

    code
    source

    /* Комментарий */

colm 	

    code
    source

    columns: ;

trf 	

    code
    source

    -webkit-transform: ;
    -moz-transform: ;
    -ms-transform: ;
    -o-transform: ;
    transform: ;

trfr 	

    code
    source

    -webkit-transform: rotate(angle);
    -moz-transform: rotate(angle);
    -ms-transform: rotate(angle);
    -o-transform: rotate(angle);
    transform: rotate(angle);

trfsc 	

    code
    source

    -webkit-transform: scale(x, y);
    -moz-transform: scale(x, y);
    -ms-transform: scale(x, y);
    -o-transform: scale(x, y);
    transform: scale(x, y);

trft 	

    code
    source

    -webkit-transform: translate(x, y);
    -moz-transform: translate(x, y);
    -ms-transform: translate(x, y);
    -o-transform: translate(x, y);
    transform: translate(x, y);

tfo 	

    code
    source

    -webkit-transform-origin: ;
    -moz-transform-origin: ;
    -ms-transform-origin: ;
    -o-transform-origin: ;
    transform-origin: ;

trs 	

    code
    source

    -webkit-transition: prop time;
    -moz-transition: prop time;
    -ms-transition: prop time;
    -o-transition: prop time;
    transition: prop time;

trsde 	

    code
    source

    -webkit-transition-delay: time;
    -moz-transition-delay: time;
    -ms-transition-delay: time;
    -o-transition-delay: time;
    transition-delay: time;

trsdu 	

    code
    source

    -webkit-transition-duration: time;
    -moz-transition-duration: time;
    -ms-transition-duration: time;
    -o-transition-duration: time;
    transition-duration: time;

trsp 	

    code
    source

    -webkit-transition-property: prop;
    -moz-transition-property: prop;
    -ms-transition-property: prop;
    -o-transition-property: prop;
    transition-property: prop;

us 	

    code
    source

    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;

В некоторые CSS сокращения можно подставлять свои значения, например:

    code
    source

    /* mt20 */
    .class{
        margin-top: 20px;
    }

    /* fsz20 */
    .class{
        font-size: 20px;
    }

    /* p15 */
    .class{
        padding: 15px;
    }

