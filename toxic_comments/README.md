# Классификация комментариев

## Данные

В наличии были следующие данные о комментариях:
- текст комментария;
- признак токсичного комментария.

## Задача

Построить модель для классификации комментариев на позитивные и негативные.

## Используемые библиотеки
*NLTK, skikit-learn, numpy, pandas, matplotlib*

## Решение

На основе данных о комментариях пользователей было проведено обучение трех моделей: логистическая регрессия, случайный лес и градиентный бустинг для относения комментария к категории "токсичные". Для каждой модели были определены гиперпараметры, позволяющие добиться лучшего значения F1-меры.

Наилучшее качество на валидации показала модель логистической регрессии со значениями гиперпараметров C = 10.0 и penalty = "l2". На тестовой выборке модель обучения достигла значения метрики F1 = 0.76, что удовлетворяет условиям исследования.
