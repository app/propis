propis
======

Патч, "локализующий" [devel версию coffee-script](https://github.com/michaelficarra/CoffeeScriptRedux)

В результате получаем современный язык программирования, основанный на русском языке.  
Идем, так сказать, по стопам создателей Рапиды, Аналитика, Глагола, ЯМБ и 1С :)  
Смотри также http://en.wikipedia.org/wiki/Non-English-based_programming_languages

Рабочее название языка - "Пропись".

### Процедура сборки из исходников (зависимости - ниже)

	git clone https://github.com/michaelficarra/CoffeeScriptRedux.git
	git clone https://github.com/app/propis.git
	cd CoffeeScriptRedux
	git co -b propis 2f11e6a
	npm install
	make -j
	git apply ../propis/*.patch
	make -j parser

### Запуск тестов

    node_modules/.bin/mocha --compilers coffee:. -u tdd -R dot


### Зависимости
Необходимо установить nodejs и npm (последний может быть частью первого)
Смотри ["Установка node.js через менеджер пакетов"](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)
