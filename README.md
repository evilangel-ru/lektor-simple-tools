# lektor-simple-tools
Set of simple but handy code snippets to use with [Lektor](https://www.getlektor.com/)

## Matching a noun to a numeral
See  [match_noun_to_numeral](/match_noun_to_numeral). This is useful mostly for the Russian language, so I describe it in Russian below.

Иногда вам надо написать что-то вроде "За прошлый год наш оборот составил 110 222 рубля." Здесь показан пример согласования единицы измерения (рубль) с числом. То есть в зависимости от числа будет подставлено согласованное существительное. 110 221 рубль, 110 222 рубля, 110 225 рублей. 

Если вы используете механизм ["переводов"](https://www.getlektor.com/docs/content/alts/) нужно установить плагин [jinja-content](https://www.getlektor.com/plugins/lektor-jinja-content/). Тогда вы сможете сделать это непосредственно в файле содержания только для нужного вам языка (наример contents+ru.lr), не затрагивая файлы других языков. 
В данном примере число хранится в ["мешке данных"](https://www.getlektor.com/docs/content/databags/) и подставляется в шаблон автоматически. Это полезно, если на вашей странице много чисел, и вы формируете файл с ними автоматически.
