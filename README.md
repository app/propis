propis
======

Патч, локализующий devel версию coffee-script
https://github.com/michaelficarra/CoffeeScriptRedux

В результате получаем современный язык программирования основанный на русском языке.
Идем, так сказать, по стопам создателей Рапиды, Аналитика, Глагола, ЯМБ и 1С :)
Смотри также http://en.wikipedia.org/wiki/Non-English-based_programming_languages

Рабочее название языка - "Пропись".

### Процедура сборки из исходников

	git co https://github.com/michaelficarra/CoffeeScriptRedux.git
	git co https://github.com/app/propis.git
	cd CoffeeScriptRedux
    git co -b propis 46e88ab
    make -j
	git apply ../propis/*.patch
    make -j parser

### Запуск тестов

    node_modules/.bin/mocha --compilers coffee:. -u tdd -R dot
