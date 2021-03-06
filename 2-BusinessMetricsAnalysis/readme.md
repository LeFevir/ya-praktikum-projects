# Анализ бизнес-показателей Яндекс.Афиши

Результаты в [PDF](BusinessMetricsAnalysis.pdf)

## Описание проекта

По условию задачи нужно проанализировать данные о посещениях сайта, выгрузка заказов и статистика рекламных расходов за период с июня 2017 года по май 2018 года. Нужно изучить как люди пользуются продуктом, когда они начинают покупать, сколько денег приносит каждый клиент и когда он окупается. **Цель исследования - помочь маркетологам оптимизировать маркетинговые затраты**.

## Использованные технологии и библиотеки

Python, pandas, matplotlib, seaborn

## Использованные аналитические инструменты

1. Исследовательский анализ исходных данных (EDA).
2. Когортный анализ пользователей и покупателей.
3. Расчет и анализ метрик пользовательской активности: частота заходов, продолжительность сессий, частота возвращений (DAU, WAU, ASL, retention rate).
4. Расчет и анализ метрик продаж (когда начинают покупать, средний чек, LTV, конверсия).
5. Расчет и анализ маркетинговых метрик: стоимость привлечения, метрики по каналам привлечения, возврат на инвестиции (CAC, ROI, ROMI).

## Основные выводы

По результатам анализа на текущий момент затраты на маркетинг не окупаются. В то же время, благодаря запуску типа источника покупателей 3 в августе 2017 года количество покупателей выросло практически в 3 раза, что сразу дало показатель окупаемости свыше 1 в сентябре. В то же время, дальнейшие затраты на этот источник трафика не принес результата в связи с довольно низким средним чеком, что не дает окупиться затратам на привлечение клиентов. Было бы логично испробовать другие источники трафика и увеличить их финансирование за счет источника 3.

Так как больше всего пользователей приходят с настольных систем и только малая часть со смартфонов, стоит дополнительно рассмотреть маркетинговые акции и способы привлечения, нацеленные на пользователей смартфонов, так как, возможно, еще не исчерпан предел пользователем, которым был бы интересен сервис с мобильных устройств. В то же время, среднее время сессии на мобильных устройствах ниже и количество визитов также ниже, чем для настольных систем.

С учетом показателей метрики LTV валовой прибыли с клиента и низкой доли возвращающихся клиентов стоит рассмотреть дополнительные маркетинговый акции, направленные на удержание клиента (например, бонусная программа). Как показывает анализ затраты на привлечение пользовательских когорт могут окупаться спустя несколько месяцев, поэтому очень важно привлекать клиентов, которые уже попробовали продукт.

Как показал анализ, на конец выборки окупились источники 1, 2, 5 и 9. С точки зрения использования маркетингового бюджета стоит сохранить канал привлечения 1, но сократить расходы на каналы 3 и 4, так как их привлечение не окупается, а больше всего средств расходуется на канал 3. 4 канал в долгосрочной перспективе смог бы окупится, но он требует слишком большого бюджета, а ROMI растет слишком медленно. Каналы 6, 7, 8 практически не принесли новых заказов, но и бюджет на них был минимален. Стоит внимательнее отнестись к этим источникам, так как они могут как являться точкой потенциального роста, так и просто привлекать не ту аудиторию и развивать их не имеет смысла. Источник 10 показал стабильный результат, но за счет того, что бюджет на него не изменялся, возможно не смог раскрыть весь свой потенциал.
