# Использование алгоритмов машинного обучения для предсказания потребности в медицинских услугах в различных регионах (Лабораторная №1)

# Цель лабораторной работы:
Исследовать и провести анализ данных медицинских расходов с использованием алгоритмов машинного обучения для предсказания потребности в медицинских услугах в различных регионах. Конкретные задачи могут включать в себя:

Исследование структуры данных: Провести разведочный анализ данных (EDA), включая изучение распределения признаков, корреляций между ними, анализ выбросов и т.д.

Визуализация данных: Использовать графические методы для визуализации зависимостей между различными переменными, чтобы получить инсайты и представление о структуре данных.

Статистический анализ: Применить статистические методы для проверки гипотез и выявления взаимосвязей между переменными.

Множественная линейная регрессия: Построить модель множественной линейной регрессии для предсказания медицинских расходов, используя различные признаки, такие как возраст, ИМТ и количество детей.

Модель предсказания на основе курения: Использовать модель машинного обучения (линейной регрессии) для предсказания медицинских расходов в зависимости от курения.

Оценка качества модели: Оценить качество модели с использованием метрик, таких как R-squared, чтобы определить, насколько успешно модель предсказывает медицинские расходы.

Выводы и рекомендации: Сформулировать выводы на основе анализа данных и результатов моделирования, предложить рекомендации или дополнительные шаги для улучшения предсказательной модели.

Лабораторная работа в данном случае предполагает практическое применение методов анализа данных и машинного обучения для извлечения информации из предоставленного набора данных и получения инсайтов в области медицинских расходов.
# Использование
**Kaggle**
https://www.kaggle.com/code/timka01/the-need-for-medical-services/edit/run/156567718

Чтобы использовать этот код и провести эксперименты с различными функциями активации, выполните следующие шаги:
Скачть датасет под названием insurance.csv, который находиться выше.

**Загружаем датасет**
![image](https://github.com/TimerbaevF/-/assets/114729066/64ec34c8-2d97-4311-8cce-cac243685ce7)

**Имортируем библиотеки**
![image](https://github.com/TimerbaevF/-/assets/114729066/a845ee8f-4981-4d17-90f7-0c8c19cc5755)

**Считываем датасет**
![image](https://github.com/TimerbaevF/-/assets/114729066/ea17d3a6-bd45-4f82-b88b-4a3cf3735e35)

# Запускать код по порядку
**https://www.kaggle.com/code/timka01/the-need-for-medical-services/edit/run/156567718**
# Библиотеки
(Эти библиотеки предоставляют мощные средства для обработки данных, визуализации результатов и построения и оценки моделей машинного обучения)

  **NumPy (import numpy as np):**
Цель использования: NumPy предоставляет функциональность для работы с многомерными массивами и матрицами, что делает его основной библиотекой для выполнения операций линейной алгебры в Python.

  **Pandas (import pandas as pd):**
Цель использования: Pandas предоставляет структуры данных и функции для эффективной работы с табличными данными. DataFrame в Pandas используется для хранения и манипуляции данными.

  **Matplotlib (import matplotlib.pyplot as plt):**
Цель использования: Matplotlib используется для создания визуализаций данных. В данном коде используется для построения различных графиков, таких как pair plot, bar plot, scatter plot и т.д.

  **Seaborn (import seaborn as sb):**
Цель использования: Seaborn — это библиотека для красивой визуализации данных на основе Matplotlib. Она упрощает создание информативных и привлекательных графиков. В коде используется для создания pair plot, bar plot, heatmap и других графиков.

  **Statsmodels (import statsmodels.api as sm):**
Цель использования: Statsmodels предоставляет классы и функции для оценки статистических моделей. В данном коде используется для выполнения множественной линейной регрессии с использованием метода OLS (Метод наименьших квадратов).

  **Scikit-Learn (from sklearn...):**
Цель использования: Scikit-Learn предоставляет множество инструментов для машинного обучения и анализа данных. В коде используется для разделения данных на обучающие и тестовые наборы, стандартизации значений, обучения линейной регрессии и оценки качества модели.
# Методы и модели, реализованные в коде

 1 **Методы анализа данных:**
Отображение данных: Импорт и отображение основных столбцов из набора данных, включая возраст, пол, ИМТ, количество детей, информацию о курении, регион проживания и медицинские расходы.
Описательная статистика: Вывод описательной статистики, включая среднее, медиану, стандартное отклонение и квартили для каждого числового столбца.

 2 **Визуализация данных:**
Pair Plot: Построение pair plot для визуального анализа взаимосвязей между различными числовыми признаками в зависимости от количества детей.
Bar Plot: Построение bar plot, показывающего количество курильщиков по регионам.
Bar Plot: Построение bar plot, показывающего распределение числа детей пациентов в зависимости от возраста и пола.
Scatter Plot: Построение scatter plot для оценки влияния возраста на медицинские расходы.
Scatter Plot: Построение scatter plot для анализа распределения ИМТ в зависимости от возраста и пола.
Heatmap: Построение тепловой карты для визуализации корреляции между числовыми признаками.

 3 **Статистический анализ:**
Множественная линейная регрессия: Использование библиотеки Statsmodels для выполнения множественной линейной регрессии с использованием метода наименьших квадратов (OLS).

 4 **Машинное обучение:**
Linear Regression (Scikit-Learn): Использование библиотеки Scikit-Learn для построения и обучения модели линейной регрессии для предсказания медицинских расходов в зависимости от курения.

 5 **Оценка качества модели:**
R-squared: Вычисление значения R-squared для оценки качества предсказаний модели.
## Результаты и Выводы

1 **Характеристики данных:**
Набор данных включает информацию о возрасте, поле, индексе массы тела (ИМТ), количестве детей, курении, регионе проживания и индивидуальных медицинских расходах.
Пропущенных значений в данных не обнаружено.

2 **Влияние факторов на медицинские расходы:**
Проведен анализ влияния различных факторов на медицинские расходы, включая возраст, ИМТ, количество детей и курение.
Построены графики и графики, чтобы визуально оценить взаимосвязи между различными признаками и медицинскими расходами.

3 **Множественная линейная регрессия:**
Проведена множественная линейная регрессия с использованием метода наименьших квадратов.
Выявлены статистически значимые зависимости между возрастом, ИМТ и количеством детей и индивидуальными медицинскими расходами.

4 **Модель машинного обучения:**
Использована модель линейной регрессии для предсказания медицинских расходов в зависимости от курения.
Оценена модель с использованием метрики R-squared, которая показала приемлемую предсказательную способность.

5 **Выводы:**
Медицинские расходы значительно коррелируют с возрастом, ИМТ и количеством детей, что подтверждено как множественной линейной регрессией, так и моделью машинного обучения.
Курение также оказывает влияние на уровень медицинских расходов, как показано в модели машинного обучения.
Регион проживания не был включен в анализ из-за удаления этого столбца перед множественной линейной регрессией.

6 **Рекомендации:**
Дополнительные исследования могут включать в себя учет других факторов, таких как стиль жизни, наличие хронических заболеваний и др., для более точного предсказания медицинских расходов.
Рекомендуется провести более глубокий анализ влияния региона проживания на медицинские расходы, возможно, с использованием дополнительных методов и моделей.
Для улучшения качества модели можно рассмотреть включение дополнительных признаков и тщательную настройку параметров модели.
