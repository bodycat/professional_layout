# professional_layout
GeekBrains HTML/CSS

Teacher:
Igor Kubikov

ПО
http://instant-eyedropper.com/

https://www.gimp.org/downloads/

https://winscp.net/eng/docs/lang:ru

БЫСТРАЯ НАСТРОЙКА SUBLIME TEXT 3 ДЛЯ РАБОТЫ:

Установка модулей на Sublime Text 3:
https://www.youtube.com/watch?v=qlueo6wFikM&feature=youtu.be
В редакторе жмите Ctrl+ или 
View -> Show console 
Если у вас русифицированный Sublime Text 3, то 
Вид -> Показать/скрыть консоль. После этого откроется панель ввода, вставьте в нижнюю строку код.

import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 

Перезапустить редактор. После установки, Package Control будет доступен в меню 
Preferences - Package Control

УСТАНОВКА ПЛАГИНОВ:


Рассмотрим на плагине Emmet.

Нажать на «Preferences» (Глобальные параметры) или Ctrl + Shift + P и в самом низу кликнуть на Package Control, у вас всплывет окно, нажимайте на «Install Package» (Установить Пакет) на шестой строке.

После этого всплывет еще одно окно где нужно ввести слово «Emmet», появится много предложений и словосочетаний, 
нажать на самую первую надпись.

СТАВИМ ТЕМНУЮ ТЕМУ:
Preferences -> Color Scheme -> Monokai

ПЛАГИНЫ ДЛЯ РАБОТЫ:
Preferences > Package Settings ->

BracketHighlighter

ColorHighlight

CSSTidy

Emmet - ускоряет написание HTML и CSS кода до скорости света. 

Урок по Emmet: https://www.youtube.com/watch?v=RfFtACtO998

https://webdesign-master.ru/blog/html-css/2.html

HTMLBeautyfy
Устраняет клингонский акцент в коде.

Package Control

Side Bar

SublimeInSaveBuild

Tagify

LiveReload
Позволяет автоматически перезагружать страничку в браузере

SublimeREPL

ColorPicker
https://www.youtube.com/watch?v=t1xZ0v5pBPY

AutoFileName - дополняет код при написании путей до файлов в вёрстке

Gist - подключает в Sublime Text возможность использовать сервис сниппетов кода GitHub Gist. 
Урок по Gist: https://www.youtube.com/watch?v=fUUXus8gGk0

Sass - плагин для подсветки Sass синтаксиса в Sass и Scss файлах. Раскрывает Emmet в Sass файлах.

Editorconfig - универсальный конфиг для всех редакторов

Autoprefixer
https://www.youtube.com/watch?v=HLg2VgFPCFc

SFTP

JAVA SCRIPT

JS Lint
https://habr.com/ru/post/242623/

AngularJS
Добавляет подсказки при вводе Angular-директив. 
