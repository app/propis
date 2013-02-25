propis
======

Патч, "локализующий" devel версию coffee-script
https://github.com/michaelficarra/CoffeeScriptRedux

В результате получаем современный язык программирования основанный на русском языке.
Идем, так сказать, по стопам создателей Рапиды, Аналитика, Глагола, ЯМБ и 1С :)
Смотри также http://en.wikipedia.org/wiki/Non-English-based_programming_languages

Рабочее название языка - "Пропись".

### Процедура сборки из исходников (зависимости - ниже)

  git clone https://github.com/michaelficarra/CoffeeScriptRedux.git
  git clone https://github.com/app/propis.git
  cd CoffeeScriptRedux
  git co -b propis 9895cd1
  npm install
  make -j
  git apply ../propis/*.patch
  make -j parser

### Запуск тестов

    node_modules/.bin/mocha --compilers coffee:. -u tdd -R dot


### Зависимости

Зависимости для Ubuntu 12.10
Перед началом сборки необходимо установить
nodejs (проверено для 0.8.16) и npm (проверено для 1.1.69)
например из репозитария https://launchpad.net/~chris-lea/+archive/node.js/


