# Shishka Timing Prediction

## Описание проблемы

...

## Описание стека использованных технологий

Для анализа набора данных (далее - датасета), визуализации и выявления паттернов, а также для создания модели предсказывания даты окончания задачи был использован следующий стек технологий:

<img src="/docs/pics/Frame18.png" alt="Python" width="75"/>
Python - это высокоуровневый язык программирования общего назначения с динамической строгой типизацией и автоматическим управлением памятью, ориентированный на повышение производительности разработчика, читаемости кода и его качества, а также на обеспечение переносимости написанных на нём программ.

---

<img src="/docs/pics/Frame17.png" alt="Pandas" width="75"/>
NumPy - это фундаментальная библиотека для математических вычислений, анализа данных и работы с n-мерными масивами, матрицами и формулами. 

---

<img src="/docs/pics/Frame19.png" alt="NumPy" width="75"/>
Pandas - это быстрый, мощный, гибкий и простой в использовании инструмент анализа данных с открытым исходным кодом и манипулирования ими, построенный на основе языка программирования Python.

---

<img src="/docs/pics/bamboolib.png" alt="Bamboolib" width="75"/>
Bamboolib - это графический интерфейс для работы с данными совместно с фреймворком Pandas. Благодаря нему появляется возможность оценивать информативность критериев и проводить поиск зависимостей, благодаря автоматическому построению графиков и диаграмм.

---

<img src="/docs/pics/Frame8.png" alt="StatsModels" width="75"/>
Statsmodels - это библиотека для статистического анализа данных на языке Python. Она предоставляет широкий спектр функций для выполнения различных задач, связанных с анализом данных, включая регрессионный анализ, прогнозирование временных рядов, анализ дисперсии и многое другое.

---

<img src="/docs/pics/Frame7.png" alt="ImbLearn" width="75"/>
Imbalanced-learn (imblearn) - это библиотека Python, которая предоставляет инструменты для работы с данными, которые имеют дисбаланс классов. Она предоставляет различные методы для балансировки классов, такие как SMOTE, ADASYN, RUSBoost, EasyEnsemble и другие. Библиотека также содержит инструменты для оценки качества модели, такие как ROC-AUC и Precision-Recall.

---

<img src="/docs/pics/Frame11.png" alt="CatBoost" width="75"/>
CatBoost - это библиотека машинного обучения, разработанная в России компанией Yandex. Она использует алгоритмы градиентного бустинга и работает с категориальными и числовыми признаками. CatBoost имеет ряд преимуществ перед другими библиотеками машинного обучения.


## Поиск фич и выявление паттернов 

...

## Описание модели

...

## Реализация UI/UX интерфейса

Для реализации пользовательского интерфеса, отражающего примерный вариант использования модели, мы использовали:

<img src="/docs/pics/Frame6.png" alt="FastAPI" width="75"/>
FastAPI - это фреймворк для создания веб-приложений на языке Python, который позволяет создавать быстрые и масштабируемые API. Он основан на принципах RESTful API, что делает его удобным для разработки веб-сервисов.
FastAPI использует асинхронное программирование и может работать с различными базами данных, такими как PostgreSQL, MySQL, SQLite и другими. Он также поддерживает интеграцию с популярными фреймворками, такими как Django, Flask и Pyramid.
Одним из главных преимуществ FastAPI является его простота в использовании. Он имеет понятный и лаконичный API, который легко понять и использовать. Кроме того, FastAPI имеет встроенную поддержку документации, что упрощает разработку и сопровождение веб-приложения.
расскажи что такое react

---

<img src="/docs/pics/Frame14.png" alt="React" width="75"/>
React - это библиотека JavaScript для создания пользовательских интерфейсов, которая позволяет создавать интерактивные и динамические веб-приложения. Она основана на концепции компонентов, которые представляют собой блоки кода, которые могут быть повторно использованы и переиспользованы в разных частях приложения. React позволяет создавать сложные интерфейсы, используя компоненты, которые взаимодействуют друг с другом и могут изменять состояние приложения в зависимости от действий пользователя.

---
Демонстрацию решения и GUI можете посмотреть [здесь](https://disk.yandex.ru/d/-GxHA0RTZsguxQ)

Более подробное описание реализации интерфеса веб-приложения можно найти [здесь](https://github.com/zayycev22/shishka_oracle)

## Инструкция по коду
Первоначально нужно создать папку files и скачать туда файлы из папки train files на Яндекс Диске

1. Первым запускается ноутбук parse.ipynb, создается новый датасет под названием pred_final.csv
2. После запускается parse2.ipynb, там содается новый dataset под названием timelines.csv (Запускается только в том случае, если нужно заново обучиться, представлена уже обученная модель cat_model)
3. Запускаем ans_predictor.ipynb, там уже стоит название файла датасета, который мы получили из 1 шага, просто запускаем и все
