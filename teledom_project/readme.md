# Проект для компании "ТелеДом" (предсказание оттока клиентов)
Оператор связи «ТелеДом» хочет бороться с оттоком клиентов. Для этого его сотрудники начнут предлагать промокоды и специальные условия всем, кто планирует отказаться от услуг связи. Чтобы заранее находить таких пользователей, «ТелеДому» нужна модель, которая будет предсказывать, разорвёт ли абонент договор. Моей задачей было обучить модель для прогноза оттока клиентов.\
В рамках работы над данным проектом:
- Была проведена предобработка данных. Объединение таблиц
- Исследовательский анализ данных
- Написан пайплайн в целях перебора моделей и гиперпараметров. Используемые модели можно посмотреть в стеке технологий
- Была оценена важность признаков при помощи библиотеки `shap`
- Построена матрица ошибок
Далее был проведён анализ полученных результатов и даны рекомендации бизнессу.\

При моделировании и принятии бизнесс-решений:
- Длительность договора сильнее всего влияет, так что стоит задуматься о каких-то предложениях для лучшего удержания новых абонентов и специальные предложения для "старичков", чтобы они продолжали пользоваться услугами компании.
- Меньше уделять внимания личным подробностям абонента: пенсионер, есть ли дети. Это оказывает наименьшее влияние
- Количество расходов (суммарное, ежемесячное) тоже оказывает влияние: можно задуматься о каких-либо предложениях, в целя уменьшения расходов с минимальными потерями для компании

## Стек технологий
`python`, `pandas`,  `matplotlib`, `numpy`, `seaborn`, `phik`, `sklearn`(Линейные/древесные модели для классификации, `RandomForestClassifier`, метрики, масштабирование и кодирование данных. Написание пайплайнов в целях перебора гиперпараметров и определения лучшей модели), `CatBoostClassifier`, анализ важности признаков при помощи `shap`.
