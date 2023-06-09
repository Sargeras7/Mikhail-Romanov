### Описание проекта

В данном  проекте  мы анализируем бизнес-показатели  стартапа, который продаёт продукты питания. Объектом исследования являются пользователи мобильного приложения, а субъектом их поведение во время его использования. Нам необходимо изучить воронку продаж, узать как пользователи доходят до покупки, их конверсию на каждом этапе от ознакомления с приложением, до собственно, покупки, а также сколько пользователей отсеиваются на каждом этапе.  

1. Изучение общей информации
- Путь к файлу: /datasets/logs_exp.csv
2.  Подготовка данных к анализу
- Привести названия стоблцов к змеиному регистру
- Проверим пропуски и типы данных. Привдем данные к необходимому для анализа формату. 
3. Изучение и проверка данных
- Сколько всего событий в логе?
- Сколько всего пользователей в логе?
- Сколько в среднем событий приходится на пользователя?
- Данными за какой период мы располагаем? Найдём максимальную и минимальную дату. Построим гистограмму по дате и времени. Можно ли быть уверенным, что у нас одинаково полные данные за весь период? Технически в логи новых дней по некоторым пользователям могут «доезжать» события из прошлого — это может «перекашивать данные». Определим, с какого момента данные полные. Данными за какой период времени мы располагаем на самом деле?
- Много ли событий и пользователей мы потеряли, отбросив старые данные?
- Проверим, что у нас есть пользователи из всех трёх экспериментальных групп.
4. Изучение воронки событий
- Посмотрим, какие события есть в логах, как часто они встречаются.
- Посчитаем, сколько пользователей совершали каждое из этих событий. Посчитаем долю пользователей, которые хоть раз совершали событие.
- Предположим, в каком порядке происходят события. Все ли они выстраиваются в последовательную цепочку?
- По воронке событий посчитаем, какая доля пользователей проходит на следующий шаг воронки (от числа пользователей на предыдущем). То есть для последовательности событий 1 →2 → 3 посчитаем отношение числа пользователей с событием 2 к количеству пользователей с событием 1, а также отношение числа пользователей с событием C к количеству пользователей с событием 2.
- На каком шаге теряем больше всего пользователей?
- Какая доля пользователей доходит от первого события до оплаты?
5. Изучение результатов эксперимента
- Определить, сколько пользователей в каждой экспериментальной группе?
- Проверить корректность всех механизмов и расчётов. Проверим, находят ли статистические критерии разницу между выборками 246 и 247.
- Выберем самое популярное событие. Посчитаем число пользователей, совершивших это событие в каждой из контрольных групп. 
- Посчитаем долю пользователей, совершивших это событие. 
- Проверим, будет ли отличие между группами статистически достоверным. 
- Проделаем то же самое для всех других событий и сделаем вывод о корректности   разбиения на группы.
- Провести те же операции с эксперементальной группой ( группой с изменённым шрифтом). 
- Сравним результаты с каждой из контрольных групп в отдельности по каждому событию. 
- Сравним результаты с объединённой контрольной группой.
6. Вывод
- Сформулируем итоговый вывод
