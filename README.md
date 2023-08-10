# Портфолио: аналитик данных

## Обо мне 

Привет! Меня зовут Илья, и Вы попали на мой прекрасный репозиторий!<br>
Я начинающий аналитик данных, и здесь я поделюсь с Вами  проектами, которыми я занимался во время своего обучения и практики!

<br>

## Навыки и технологии
- Инструменты анализа данных: ``SQL``, ``Excel``: 
- Языки программирования и библиотеки: ``Python``, ``Pandas``, ``math`` 
- Системы управления базами данных: ``MySQL``, ``PostgreSQL``

## Проекты
<p> Проект 1: Калькулятор юнит-экономики онлайн-школы</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1. Настроить в калькуляторе учет корректировок планов маркетинга.</li>
  <li>Задача №2. Пересчитать план найма преподавателей.</li>
</ol>

<p>Как решал: <p>
Задача №1<br>
1. Добавил в список параметров нашего калькулятора показатель "Поправочный коэф-т на привлечение"<br>
2. Установил значение этого показателя по умолчанию как 100% и добавил возможность изменять этот показатель для расчётного периода 05.21-04.22 по аналогии с другими - через столбец "Изменение"<br>
3. Настроил динамический расчёт количества новых студентов за период 05.21-04.22 с поправкой на этот коэффициент. Если для 05.21-04.22 он равен 120%, то в каждый месяц этого периода рассчётное значение количества новых студентов должно быть больше на 20%<br>
4. Просчитал сценарий, при котором планы маркетинга будут увеличены на 12% (настройки остальных показателей не меняются)<br>
<br>
Задача №2<br>
1. Добавил в калькулятор Найма преподавателей возможность изменять входных параметры: Пропускную способность П и Retention П - с помощью дополнительного столбца с процентными изменениями, как это сделано на Главном листе с основным калькулятором Юнит-экономики<br>
2. Сделал поправку в расчёте общей пропускной способности - изменил формулу так, чтобы отразить, что новые преподаватели в первый месяц своей работы могут проводить только половину уроков от средней пропускной способности преподавателя, задаваемой параметром<br>
3. Обновил прогнозное количество уроков, добавив новые значения из Задачи 1 (полученные после поправки на планы маркетинга)<br>
4. Просчитал сценарий, при котором Пропускная способность П увеличится на 15 процентов, а Retention П упадёт на 2 процента<br>
5. С помощью Поиска решений составил новый план найма с ограничением: за месяц нельзя нанять более 70 преподавателей<br>
<br>



> <a href="https://github.com/degtyarev-ilya/degtyarev.ilya/blob/main/%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%20%E2%84%961.xlsx">Ссылка на проект</a>


<p>Выводы (итоги):<p>
<ol>
  <li>Итог №1: Обновленный лист с калькулятором + новое расчётное количество студентов на 04.2022</li>
  <li>Итог №2: Обновлённый план по найму - с количеством новых преподавателей по месяцам за период с 05.2021 по 04.2022</li>
</ol>
<br> 

<p> Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1. Определить, что является юнитом в нашей экономике.</li>
  <li>Задача №2. Посчитать юнит-экономику продукта и предложить сценарий по настройке параметров для выхода на 25%-ную маржинальность.</li>
  <li>Задача №3. Выбрать оптимальный вариант расчета Retention</li>
  <li>Задача №4. Собрать визуализации основных бизнес-показателей.</li>
  <li>Задача №5. Исследовать данные о пользователях и их поведении.</li>
</ol>

<p>Как решал:<p>
1. Агрегировал сырые данные, чтобы получить сводные показатели для расчета юнит-экономики<br>
2. Посчитал необходимые бизнес-показатели<br>
3. Визуализировал распределение, поизучал данные в целом на предмет каких-то взаимосвязей, закономерностей. Обратил внимание на то, сколько времени пользователи проводят на платформе, посмотрел, как распределены всплески активностей по сезонам и дням.<br>

> <a href="https://github.com/degtyarev-ilya/degtyarev.ilya/blob/main/%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%20%E2%84%962.xlsx">Ссылка на проект</a>

 
<p>Выводы (итоги):<p>
<ol>
  <li>Итог №1: Визуализированы распределение подписчиков по часовым поясам</li>
  <li>Итог №2: Лист с калькулятором + Визуализация бизнес-показателей</li>
</ol>
<br> 

<br> 
<p> Проект 3: Когортный анализ онлайн-кинотеатра с помощью SQL</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1. Построить распределение количества первых покупок клиента</li>
  <li>Задача №2. Отобразить винтажные доходимости для каждого партнера </li>
</ol>

<p>Как решал:<p>
1. Перешел на схему course_db_main и изучите информацию, которая хранится в таблице skycinema.client_sign_up.<br>
2. Проставил каждой покупке свой ранг, который покажет, какой по счету является данная покупка в рамках всей таблицы.<br>
3. Проставил каждой покупке свой ранг, который покажет, какой по счету является данная покупка в рамках всех покупок клиента.<br>
4. Рассмотрел только первые покупки для каждого клиента.<br>
5. Дополнил код таким образом, чтобы получились винтажные доходимости, отобразив какой процент клиентов дошел до второй покупки, до третьей покупки и т. д.<br>

> <a href="https://github.com/degtyarev-ilya/degtyarev.ilya/blob/main/%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%20%E2%84%963.txt">Ссылка на проект</a>

  <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1. Узнал, какой партнер приносит больше клиентов</li>
  <li>Итог №2. Узнал, какой партнер приносит больше долгосрочных клиентов</li>
</ol>

<br> 
<p>Проект 4: Построение витрины для модели машинного обучения в банке </p> 
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1. Специалисты по машинному обучению попросили составить витрину для их модели.</li>
</ol>
  
<p>Как решал:<p>
Взял таблицу skybank.late_collection_clients и написал скрипт, который сделал витрину со следующими полями:<br>
  <ol>
1) Внутренний идентификатор клиента — поле id_client.<br>
2) Название города — поле name_city из таблицы skybank.region_dict.<br>
3) Числовой признак, который принимает значение 1 для мужчин и 0 для женщин — новое поле nflag_gender на основании поля gender.<br>
4) Возраст — поле age.<br>
5) Числовая переменная, которая показывает, в первый ли раз клиент обратился к нам за кредитом, — поле first_time.<br>
6) Числовой признак, который принимает значение 1 при наличии мобильного телефона и 0 при его отсутствии — новое поле nflag_cellphone на основании поля cellphone.<br>
7) Числовая переменная, которая показывает, активен ли клиент, — поле is_active<br>
8) Номер клиентского сегмента — поле cl_segm.<br>
9) Размер выданного кредита — поле amt_loan.<br>
10) Дата выдачи кредита — поле date_loan. Необходимо привести к формату даты.<br>
11) Тип выданного кредита — поле credit_type.<br>
12) Суммарный объем кредитов, выданных в этом городе.<br>
13) Доля данного кредита среди всех кредитов, выданных в этом городе.<br>
14) Суммарный объем кредитов, выданных в рамках указанного типа кредита.<br>
15) Доля данного кредита среди всех кредитов, выданных в рамках указанного типа кредита.<br>
16) Суммарный объем кредитов, выданных в рамках указанного типа кредита и города.<br>
17) Доля данного кредита среди всех кредитов, выданных в рамках указанного типа кредита и города.<br>
18) Количество кредитов, выданных в этом городе.<br>
19) Количество кредитов, выданных в рамках указанного типа кредита.<br>
20) Количество кредитов, выданных в рамках указанного типа кредита и города.<br>
  </ol>

> <a href="https://github.com/degtyarev-ilya/degtyarev.ilya/blob/main/%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%20%E2%84%964%20.txt">Ссылка на проект</a>

  
 <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1: Готовая витрина для модели машинного обучения в банке</li>
</ol>
<br> 


<p>Проект 5: Моделирование изменения балансов студентов</p> 
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1. Выяснить, сколько всего уроков было на балансе всех учеников за каждый календарный день</li>
  <li>Задача №2. Выяснить, как это количество менялось под влиянием транзакций (оплат, начислений, корректирующих списаний) и уроков (списаний с баланса по мере прохождения уроков), другими словами, создать таблицу, где будут балансы каждого студента за каждый день.</li>
</ol>

<p>Как решал<p>
1. Узнал, когда была первая транзакция для каждого студента. Начиная с этой даты, собирал баланс уроков. <br>
2. Создал CTE `first_payments` с двумя полями: `user_id` и `first_payment_date` (дата первой успешной транзакции). <br>
3. Собрал таблицу с датами за каждый календарный день 2016 года. Выбрал все даты из таблицы `classes`, создал CTE `all_dates` с полем `dt`, где будут храниться уникальные даты (без времени) уроков.<br>
4. Узнал, за какие даты имеет смысл собирать баланс для каждого студента. Для этого объединил таблицы и создал CTE `all_dates_by_user`, где будут храниться все даты жизни студента после того, как произошла его первая транзакция. <br>
5. Нашел все изменения балансов, связанные с успешными транзакциями. Выбрал все транзакции из таблицы `payments`, сгруппировал их по `user_id` и дате транзакции (без времени) и нашел сумму по полю `classes`. В результате получил CTE `payments_by_dates` с полями: `user_id`, `payment_date`, `transaction_balance_change` (сколько уроков было начислено или списано в этот день).<br> 
6. Нашел баланс студентов, который сформирован только транзакциями. Для этого объединил `all_dates_by_user` и `payments_by_dates` так, чтобы совпадали даты и `user_id`. Использовал оконные выражения (функцию `sum`), чтобы найти кумулятивную сумму по полю `transaction_balance_change` для всех строк до текущей включительно с разбивкой по `user_id` и сортировкой по `dt`. В результате получил CTE `payments_by_dates_cumsum` с полями: `user_id`, `dt`, `transaction_balance_change` — `transaction_balance_change_cs` (кумулятивная сумма по `transaction_balance_change`). При подсчете кумулятивной суммы можно заменил пустые значения нулями.<br>
7. Нашел изменения балансов из-за прохождения уроков. Создал CTE `classes_by_dates`, посчитав в таблице `classes` количество уроков за каждый день для каждого ученика. Получил результат с такими полями: `user_id`, `class_date`, `classes` (количество пройденных в этот день уроков).<br>
8. По аналогии с уже проделанным шагом для оплат создал CTE для хранения кумулятивной суммы количества пройденных уроков.  Для этого объединим таблицы `all_dates_by_user` и `classes_by_dates` так, чтобы совпадали даты и `user_id`. Использовал оконные выражения (функцию `sum`), чтобы найти кумулятивную сумму по полю `classes` для всех строк до текущей включительно с разбивкой по `user_id` и сортировкой по `dt`. В результате получил CTE `classes_by_dates_dates_cumsum`с полями: `user_id`, `dt`, `classes` — `classes_cs`(кумулятивная сумма по `classes`). При подсчете кумулятивной суммы заменил пустые значения нулями.<br>
9. Создал CTE `balances` с вычисленными балансами каждого студента. Для этого объединил таблицы `payments_by_dates_cumsum` и `classes_by_dates_dates_cumsum` так, чтобы совпадали даты и `user_id`. Получил такие поля:`user_id`, `dt`, `transaction_balance_change`, `transaction_balance_change_cs`, `classes`, `classes_cs`, `balance` (`classes_cs` + `transaction_balance_change_cs`).<br>
10. Посмотрел, как менялось общее количество уроков на балансах студентов.
Для этого просуммировал поля `transaction_balance_change`, `transaction_balance_change_cs`, `classes`, `classes_cs`, `balance` из CTE `balances` с группировкой и сортировкой по `dt`.<br>

> <a href="https://github.com/degtyarev-ilya/degtyarev.ilya/blob/main/%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%20%E2%84%965.txt">Ссылка на проект</a>
 
 <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1: Готовая таблица с балансами всех студентов за год</li>
</ol>

## Контактная информация
- Тел: + 79002515504
- E-mail: degtyarev.ilya56@yandex.ru 
- Telegram: https://t.me/degilya
