propis
======

Патч, локализующий devel версию coffee-script
https://github.com/michaelficarra/CoffeeScriptRedux

В результате получаем современный язык программирования основанный на русском языке.
Идем, так сказать, по стопам создателей Рапиды, Аналитика, Глагола, ЯМБ и 1С :)
Смотри также http://en.wikipedia.org/wiki/Non-English-based_programming_languages

Рабочее название языка - "Пропись".

### Наложение патча

	git co https://github.com/michaelficarra/CoffeeScriptRedux.git
	git co https://github.com/app/propis.git
	cd CoffeeScriptRedux
	git apply ../propis/propis.patch
