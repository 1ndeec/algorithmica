---
title: Классификация
---

Рассмотрим следующую задачу. Мы работаем в банке и нам необходимо, чтобы
система определяла, сможет ли человек вовремя погасить кредит или нет.

У нас есть различная информация о человеке, так называемые **признаки
(features)**. Они бывают различных типов:

-   **Бинарные признаки**: наличие телефона.

-   **Номинальные признаки**: профессия, адрес проживания.

-   **Порядковые признаки**: образование, занимаемая должность. По сути,
    они похожи на номинальные признаки, только тут у значений признака
    имеется порядок (высшее образование ценится выше среднего и т.д.).

-   **Количественные признаки**: зарплата, возраст, количество детей в
    семье и т.п.

Ответ же к данной задаче либо **0** (человек не выплатит кредит вовремя)
и **1** (Человек выплатит кредит вовремя).

Т.е. в задаче классификации значение, которое мы хотим предсказать
(далее целевая переменная ), принадлежит конечному множеству. В нашей
задаче, например, это **{0; 1}**.

Бывают множества не только из 2 классов. Например, задача диагностики
болезни по симптомам. Тут классы --- это список болезней.

Как решается данная задача? В таких задачах нам требуется **обучающая
выборка**. Это история того, как в прошлом наши клиенты выплачивали
кредиты.

Мы знаем о них все: где они работают, сколько получают и т.п. А также
нам известно смогли они выплатить кредит или нет.

Знание того, что мы предсказываем (целевой переменной) относит задачу к
**обучению с учителем**.

Далее модель машинного обучения находит закономерности в этой выборке.
Например, если человек безработный, то скорее всего, он не выплатит
кредит вовремя и т.д.

Она запоминает эти закономерности, и когда приходит черёд узнать, а
сможет ли новый клиент заплатить кредит вовремя, модель смотрит на эти
зависимости и выдаёт ответ.

Список новых клиентов называется **тестовой выборкой**. Главное её
отличие от обучающей выборки заключается в том, что для элементов из
тестовой выборки неизвестна целевая переменная (в нашем случае --- это
выплатит клиент кредит или нет).