# Интерпретатора для си-подобного языка

Код программы проходит через несколько важных этапов - лексический анализ, синтаксический анализ, семантический анализ, конвертацию в польскую инверсную запись и лишь за тем исполнение. 

## Подробное описание

Сначала текст (код) программы  проходит через лексический анализ, где исходный код преобразуется в последовательность токенов, представляющих собой логические единицы синтаксиса. 

Затем проводится синтаксический анализ. Здесь используется метод рекурсивного спуска, позволяющий парсить выражения, управляющие структуры и функции. 

Следует семантический анализ, где выявляются семантические ошибки в коде.

Далее происходит представление программы в виде (польской инверсной записи)[https://ru.wikipedia.org/wiki/%D0%9F%D0%BE%D0%BB%D1%8C%D1%81%D0%BA%D0%B0%D1%8F_%D0%B7%D0%B0%D0%BF%D0%B8%D1%81%D1%8C], что облегчает и упрощает её исполнение.

Все ошибки логируются и/или выбрасываются в виде исключений.
