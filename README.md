# usd_rates_prediction
Построение различных моделей линейной регрессии для предсказания курса доллара

Использован датасет по динамике официального курса доллара США к рублю, полученный с сайта ЦБ: https://www.cbr.ru/currency_base/dynamics/?UniDbQuery.Posted=True&UniDbQuery.mode=1&UniDbQuery.date_req1=&UniDbQuery.date_req2=&UniDbQuery.VAL_NM_RQ=R01235&UniDbQuery.From=01.01.2017&UniDbQuery.To=31.12.2019

Цель - используя модели sklearn построить модель линейной рергрессии для наиболее точного предсказания курса.

Используется модель MLPRegressor: подготавливаются данные, определяется размер ошибки с помощью разбивки датасета на тестовую и обучающую выборки (Test set, Training set) и обучением модели, подбираются параметры для MLPRegressor так, чтобы минимизировать ошибку.


Далее пробуем улучшить результат применением ещё трёх моделей:
1. DecisionTreeRegressor
2. Ridge
3. RandomForestRegressor
