# **ПРОЕКТ 5. ПРЕДСКАЗАНИЕ ПРОДОЛЖИТЕЛЬНОСТИ ПОЕЗДКИ НА ТАКСИ**

<center> <img src = https://puzzlepalace.com.au/wp-content/uploads/2018/04/New-York-Taxi-1500-Piece-by-Jumbo.jpg alt="drawing" style="width:400px;" </center>

## **Содержание**

1. [Описание проекта](https://github.com/alkoop1/educational_projects/project_5/README.md#Описание-проекта)  
2. [Решаемая задача](https://github.com/alkoop1/educational_projects/project_5/README.md#Решаемая-задача)

    2.1 [Условия](https://github.com/alkoop1/educational_projects/project_5/README.md#Условия)

    2.2 [Метрики](https://github.com/alkoop1/educational_projects/project_5/README.md#Метрики)

    2.3 [Навыки](https://github.com/alkoop1/educational_projects/project_5/README.md#Навыки)

3. [Информация о данных](https://github.com/alkoop1/educational_projects/project_5/README.md#Информация-о-данных)  
4. [Этапы работы над проектом](https://github.com/alkoop1/educational_projects/project_5/README.md#Этапы-работы-над-проектом)  
5. [Результаты](https://github.com/alkoop1/educational_projects/project_5/README.md#Результаты)
6. [Выводы](https://github.com/alkoop1/educational_projects/project_5/README.md#Выводы)

### **Описание проекта**

- Автоматизация бизнес-процессов сервисов такси города Нью-Йорк путем создания модели машинного обучения, способной предсказывать продолжительность поездки в зависимости от различных факторов.  
- Решаемая задача была представлена в качестве `Data Science`-соревнования на платформе [Kaggle](https://www.kaggle.com/competitions/nyc-taxi-trip-duration/overview) в 2017 году с призовым фондом в $30'000.

:arrow_up:[к содержанию](https://github.com/alkoop1/educational_projects/project_5/README.md#Содержание)

### **Решаемая задача**

Последовательно пройти все этапы задачи `Data Science`: обработать, отобрать и подготовить для подачи на вход модели МО признаки поездок, обучить несколько моделей и сравнить их по значению метрики качества, выбрать лучшую, с её помощью сделать предсказание и загрузить `notebook` на страницу соревнования на платформе `Kaggle`.  

#### **Условия**

- Обработать входные данные: провести разведывательный анализ, отобрать признаки, нормализовать и подготовить на вход модели МО.
- Гипотезы и выводы сопроводить иллюстрациями.
- Обучить несколько моделей из библиотеки `sklearn`: логистическая регрессия, полномиальная регрессия, случайный лес, градиентный бустинг - и сравнить их по метрике качества.
- Построить прогноз и загрузить его на платформу `Kaggle`.

#### **Метрики**

- Для сравнения моделей используется метрика `RMSLE - Root Mean Squared Log Error`, которая вычисляется на основе целевой переменной в логарифмическом масштабе.  
- Для контроля хода выполнения проекта требуется заносить получаемые данные в специальные поля на платформе `SkillFactory`, сравнивая их с эталонными значениями.  
- Итоговый ноутбук в формате `.ipynb` не проверяется менторами `SkillFactory`, поэтому оформление ноутбука выполнено в стандартном качестве, аналогично предыдущим проектам.

#### **Навыки**

- Проведение разведывательного анализа;
- Построение диаграмм с помощью библиотеки `seaborn`, `matplotlib` и `plotly`;
- Обучение моделей и оптимизация их гиперпараметров;
- Понимание и использование метрик качества моделей;
- Работа с `Kaggle`, `Git` и `GitHub` посредством добавления отчета о проделанной работе в портфолио;
- Попрактиковать навыки использования языка разметки `MarkDown`;
- Улучшить навыки составления эффективного воспроизводимого кода на `Python` в соответствии с `PEP 8`.

:arrow_up:[к содержанию](https://github.com/alkoop1/educational_projects/project_5/README.md#Содержание)

### **Информация о данных**

- Организаторами соревнования предоставлен набор данных, содержащий информацию о поездках на жёлтом такси в Нью-Йорке за 2016 год. Первоначально данные были выпущены Комиссией по Такси и Лимузинам Нью-Йорка и включают в себя информацию о времени поездки, географических координатах, количестве пассажиров и несколько других переменных.  
- Кроме этого, для решения задачи использованы вспомогательные данные из других источников, такие как:
  - национальные праздники,
  - сведения о погоде и данные из `Open Source Routing Machine` (сервиса, позволяющего строить кратчайшие маршруты по координатам и оценивать примерную длительность маршрута).    
- Информация о признаках главного датасета с 1.5 млн поездок приведена в начале ноутбука.  
  
:arrow_up:[к содержанию](https://github.com/alkoop1/educational_projects/project_5/README.md#Содержание)

### **Этапы работы над проектом**

- Первичная обработка данных.
- Разведывательный анализ данных (`EDA`).
- Отбор и преобразование признаков.
- Решение задачи регрессии: линейная регрессия и деревья решений.
- Решение задачи регрессии: ансамблевые методы и построение прогноза.
- Загрузка предсказания на `Kaggle`.

:arrow_up:[к содержанию](https://github.com/alkoop1/educational_projects/project_5/README.md#Содержание)

### **Результаты**

- Проведена обработка данных, выполнен разведывательный анализ с использованием иллюстраций.  
- Признаки отобраны и подготовлены к подаче на вход модели.
- Обучены модели машинного обучения: `LinearRegression, Ridge, DecisionTreeRegressor, RandomForestRegressor, GradientBoostingRegressor`.
- Модели сравнены по метрике `RMSLE`, результаты сведены в таблицу, сделаны выводы.

:arrow_up:[к содержанию](https://github.com/alkoop1/educational_projects/project_5/README.md#Содержание)

### **Выводы**

- Проект позволил примерить роль `Data Scientist` в сфере транспортных перевозок:
  - провести полноценное исследование собранных данных,
  - предсказать время поездки на такси с помощью различных современных моделей,
  - отобрать наиболее точную по значению заданной метрики модель.  
- Текущий результат (примерно 473 место в рейтинге соревнования) далеко не лучший, однако последующее углубление знаний в области машинного обучения вкупе с более эвристическими приемами предварительной обработки и разведывательного анализа имеющихся данных, бесспорно, позволят улучшать положение в рейтинге подобных соревнований.  
- В ходе реализации проекта улучшены навыки разведывательного анализа, работы с моделями МО, написан воспроизводимый код на `Python` в соответствии с `PEP 8`.

:arrow_up:[к содержанию](https://github.com/alkoop1/educational_projects/project_5/README.md#Содержание)