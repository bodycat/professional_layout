https://getbootstrap.com/docs/4.0/getting-started/introduction/
https://bootstrap-4.ru/
https://getbootstrap.com/docs/4.0/layout/overview/
https://bootstrap-4.ru/docs/4.0/layout/overview/
http://htmlbook.ru/CSS/background-attachment

 Как задать фиксированное фоновое изображение:
view source
print
?
1
	body
2
	{
3
	background-image:url('smiley.gif');
4
	background-repeat:no-repeat;
5
	background-attachment:fixed;
6
	}
  
  Свойство background-attachment определяет является ли фоновое изображение фиксированным или прокручивается вместе со страницей.
Значение по умолчанию: 	scroll
Наследуется: 	нет
Версия: 	CSS1
Аргументы
Значение 	Описание
scroll 	Изображение фона прокручивается вместе с страницей. Значение по умолчанию
fixed 	Фоновое изображение зафиксировано
inherit 	Значение должно быть унаследовано от элемента родителя
