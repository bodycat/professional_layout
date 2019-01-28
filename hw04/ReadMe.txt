Links:

koala-app.com
https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass
http://rightblog.ru/2781


Компиляция SASS в Sublime Text 3

SASS — это другой препроцессор для CSS. Набирает популярность, и уже обгоняет less по распространению использования.

    Устанавливаем Ruby
    Запускаем консоль, и ставим Ruby Gem gem install sass
    Устанавливаем плагин Sass для Sublime Text
    Устанавливаем плагин Sass Build для Sublime Text
    Устанавливаем плагин SublimeOnSave для Sublime Text
    (мы же говорили о этом плагине в инструкции выше)

Теперь добавим настройки в Sublime Text Settings – Default:

{
  "filename_filter": ".(sass|scss)$",
  "build_on_save": 1
}

Также не забудьте при открытом .sass файле зайти и выбрать билд систему в Tools → Build System → SASS Compressed Теперь при сохранении .sass файла будет компилироваться .css.
