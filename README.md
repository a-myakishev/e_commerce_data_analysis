# Анализ продаж и пользователей интернет магазина   

## Overview
В этом проекте проведен анализ данных о продажах и пользователях интернет магазина:
+ Ad-hoc-анализ продаж
+ Когортный анализ retention
+ RFM-сегментация пользователей 

## Стек
![Pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=FFA500)
![Seaborn](https://img.shields.io/badge/Seaborn-444876?logo=seaborn&logoColor=white&style=for-the-badge)

## Проделанная работа
### Подготовка данных:
+ Проведел EDA
+ Изучил воронку статусов заказа и определил, какой заказ считать совершенной покупкой
### Ad-hoc-анализ:
+ Подсчитал кол-во пользователей с одной покупкой (one-time purchasers)
+ Провел анализ причин недоставки заказов, подсчитал кол-во инцидентов по каждой причине
+ Для каждого товара нашел день недели с наибольшими большими продажами
+ Подсчитал среднее недельное кол-во покупок для каждого пользователя с разбивкой по месяцам
### Когортный анализ retention:
+ Построил когортную таблицу для отображения retention
+ Выявил когорту с самым высоким retention на 3-й месяц
### RFM-сегментация:
+ Проанализировал новизну, частоту и сумму покупок у пользователей магазина
+ На основе анализа продумал подходящую систему оценок RFM с учетом особенностей данных
+ Написал функции для назначения оценок RFM в зависимости от соответствующих значений новизны, частоты и денежности
+ Написал функции для удобного отображения сегментов RFM и их распределения
+ Провел анализ RFM-сегментов

## Результаты 
+ Ad-hoc анализ показал, что в магазине ~96% пользователей совершили лишь одну покупку
+ Когортный анализ показал, что в магазине довольно низкий retention 3-го месяца (максимальный -- 0.54%)
+ Ключевые выводы RFM-анализа:
1. Довольно мало лояльных клиентов -- всего около одного процента
2. Достаточно много Перспективных клиентов -- 42%. С помощью подходящих маркетинговых активностей их можно стимулировать покупать чаще.
3. Есть существенная доля количество почти спящих клиентов -- 22.4%. На этот сегмент стоит как минимум обратить внимание.
