# professional_layout
GeekBrains HTML/CSS

Teacher:
Igor Kubikov

РАБОТА НА SUBLIME TEXT 3

Установка модулей на Sublime Text 3:
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

ПЛАГИНЫ ДЛЯ РАБОТЫ:
Preferences > Package Settings ->

Color Highlighter

CSSTidy

Emmet

HTMLBeautyfy

Package Control

Side Bar

SublimeInSaveBuild

Tagify

LiveReload

SublimeREPL

ColorPicker
