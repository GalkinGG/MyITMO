 </li></ul></li></ol><h4 id="expressions-parsing">Домашнее задание 13. Разбор выражений</h4><ol><li>
            Доработайте предыдущее домашнее задание, так что бы
            выражение строилось по записи вида
            <pre>x * (x - 2)*x + 1</pre></li><li>
            В записи выражения могут встречаться:
            <ul><li>
                    бинарные операции: 
                    умножение <code>*</code>, деление <code>/</code>,
                    сложение <code>+</code> и вычитание <code>-</code>;
                </li><li>
                    унарный минус <code>-</code>;
                </li><li>
                    переменные <code>x</code>, <code>y</code> и <code>z</code>;
                </li><li>
                    целочисленные константы в десятичной системе счисления, 
                    помещающиеся в 32-битный знаковый целочисленный тип;
                </li><li>
                    круглые скобки для явного обозначения приоритета операций;
                </li><li>
                    произвольное число пробельных символов в любом месте,
                    не влияющем на однозначность понимания формулы
                    (например, между операцией и переменной, но не внутри констант).
                </li></ul></li><li>
            Приоритет операций, начиная с наивысшего
            <ol><li>унарный минус;</li><li>умножение и деление;</li><li>сложение и вычитание.</li></ol></li><li>
            Разбор выражений рекомендуется производить
            <a href="https://ru.wikibooks.org/wiki/%D0%A0%D0%B5%D0%B0%D0%BB%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D0%B8_%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC%D0%BE%D0%B2/%D0%9C%D0%B5%D1%82%D0%BE%D0%B4_%D1%80%D0%B5%D0%BA%D1%83%D1%80%D1%81%D0%B8%D0%B2%D0%BD%D0%BE%D0%B3%D0%BE_%D1%81%D0%BF%D1%83%D1%81%D0%BA%D0%B0">методом рекурсивного спуска</a>.
            <ul><li>Алгоритм должен работать за линейное время.</li><li>Лексический анализ (токенизация) не требуется.</li></ul></li></ol><h4 id="expressions-exceptions">Домашнее задание 14. Обработка ошибок</h4><ol><li>
            Добавьте в программу, вычисляющую выражения, обработку ошибок, в том числе:
            <ul><li>ошибки разбора выражений;</li><li>ошибки вычисления выражений.</li></ul></li><li>
            Для выражения <code>1000000*x*x*x*x*x/(x-1)</code> вывод программы
            должен иметь следующий вид:
            <pre>
x       f
0       0
1       division by zero
2       32000000
3       121500000
4       341333333
5       overflow
6       overflow
7       overflow
8       overflow
9       overflow
10      overflow
            </pre>
            Результат <code>division by zero</code> (<code>overflow</code>) означает,
            что в процессе вычисления произошло деление на ноль (переполнение).
        </li><li>
            При выполнении задания следует обратить внимание на дизайн и обработку исключений.
        </li><li>
            Человеко-читаемые сообщения об ошибках должны выводиться на консоль.
        </li><li>
            Программа не должна &laquo;вылетать&raquo; с исключениями (как стандартными, так и добавленными).
        </li></ol></article><aside><header><form id="search" method="get" action="https://www.google.com/search"><input type="hidden" name="sitesearch" value="kgeorgiy.info"><input type="text" name="q" maxlength="255"><button type="submit" value="Search">&#128269;</button></form></header><nav><ol><li class="i0"><a href="#runme">ДЗ-1. Hello World</a></li><li class="i0"><a href="#sum">ДЗ-2. Сумма чисел</a></li><li class="i0"><a href="#reverse">ДЗ-3. Реверс</a></li><li class="i0"><a href="#wordstat">ДЗ-4. Статистика слов</a></li><li class="i0"><a href="#scanner">ДЗ-5. Свой сканер</a></li><li class="i0"><a href="#wspp">ДЗ-6. Статистика слов++</a></li><li class="i0"><a href="#markup">ДЗ-7. Разметка</a></li><li class="i0"><a href="#git">ДЗ-8. Git</a></li><li class="i0"><a href="#md2html">ДЗ-9. Markdown to HTML</a></li><li class="i0"><a href="#qf">ДЗ-10. Чемпионат</a></li><li class="i0"><a href="#game">ДЗ-11. Игра m,n,k</a></li><li class="i0"><a href="#expessions">ДЗ-12. Выражения</a></li><li class="i0"><a href="#expressions-parsing">ДЗ-13. Разбор выражений</a></li><li class="i0"><a href="#expressions-exceptions">ДЗ-14. Обработка ошибок</a></li></ol></nav><footer><a href="https://validator.w3.org/check?uri=referer" referrerpolicy="unsafe-url"><img src="/design/valid-html5.svg" alt="Valid HTML 5" height="31" width="88"></a></footer></aside></div></body></html>
