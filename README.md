# Прикладной анализ временных рядов
Курс по временным рядам. ИТМО. AI Talent Hub. MTS

## Формулировка задания

Построить модель прогнозирования спроса (продаж) на товары в магазине `STORE_2` офлаин-ритейлера в США. Всего в магазине 15 артикулов (товаров). Прогнозировать продажи нужно на неделю, на месяц и на квартал. В качестве дополнительной информации вам переданы данные о цене товара (меняются раз в неделю, а также о праздниках в США).

### Задание 1. 
Реализовать класс, который умеет: 

1) предобрабатывать исходные данные в удобный формат; 

2) обучаться для задачи прогнозирования; 

3) оценивать качество своих прогнозов;

4) сохранять модели и подгружать их; 

5) Прогнозировать продажи на неделю, на месяц и на квартал.

Должна быть рабочая программа, которая делает инференс (прогнозирование на произвольном тестовом датасете (аналогично тому, который есть у вас)).


### Задание 2. 
Подготовить отчёт о решении данной задачи в виде jupyter ноутбука. В отчёте, в частности, вы должны ответить на следующие вопросы:

1) Какие методы предобработки данных вы использовали?

2) Какие модели пробовали? Почему пробовали именно их?

3) Как вы проверяете качество модели? На каких данных? Какие метрики используюте? Чем обусловлен выбор именно этих метрик?

4) Какое итоговое качество модели на тестовом датасете?


## Ход работы

1. Проведено объединение данных, преобразование и разведочный анализ данных (см. `./notebooks/EDA.ipynb`)
2. Рассмотрены 3 модели для прогнозирования рядов (см. `./notebooks/models.ipynb`):
    - SARIMA
    - Fourier
    - Prophet
3. Реализован класс для прознозирования рядов (см. `./notebooks/class.ipynb`)