
# <center> Разведывательный анализ данных и построение регрессивной модели, предсказывающей рейтинг отелей </center> [English version](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#-exploratory-data-analysis-and-building-a-regression-model-that-predicts-the-rating-of-hotels--%D0%BA-%D1%80%D1%83%D1%81%D1%81%D0%BA%D0%BE%D0%B9-%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D0%B8)


## Оглавление
1. [Описание проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

1.1. [Краткая информация о данных](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%B0%D1%8F-%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)

1.2. [Этапы работы над проектом](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)
    
1.3. [Предварительные выводы](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BF%D1%80%D0%B5%D0%B4%D0%B2%D0%B0%D1%80%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

2. [Используемый зависимости](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D1%8B%D0%B5-%D0%B7%D0%B0%D0%B2%D0%B8%D1%81%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8)

3. [Установка проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

4. [Использование проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

5. [Авторы](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%B0%D0%B2%D1%82%D0%BE%D1%80%D1%8B)

6. [Результаты](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B)

## Описание проекта

**Данный проект** направлен на исследование структуры и зависимостей (разведывательный анализ)  данных, отбор и преобразование признаков для обучения модели, предсказывающей рейтинг отелей, на основе имеющихся в датасетах данных о 515 000 отзывах на отели Европы по данным сайта Booking. В качестве статистической меры использовалась **MAPE. (Mean Absolute Percentages Error)**.

# Задача:
На основе имеющихся в датасете данных о 515 000 отзывах на отели Европы обучить модель, которая должна предсказывать рейтинг отеля по данным сайта Booking. 

## Проблема:
Наличие отелей накручивающих себе рейтинг на Booking

## Цель проекта:
Построить модель на основе алгоритмов машинного обучения, которая предсказывает рейтинг отеля.

Наш проект включает в себя несколько этапов:

- отбор необходимых библиотек;
- знакомство с исходными данными;
- подготовка данных, которые будут использованы для обучения модели;
- отбор признаков;
- создание и обучение модели;
- оценка эффективности модели;
-  предсказание моделью результатов по тестовым данным;
- подготовка сабмишна;
- отправка результатов на соревнование в Kaggle;
- подготовка и выгрузка проекта в GitHub.

** О структуре проекта:**

* [Сабмишн](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/submission.csv)
* [Ноутбук с кодом/Booking_model.ipynb](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/booking_model.ipynb)
* [Папка с данными](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model/data)  датасет с тестовыми данными (hotels_test.csv.zip) и датасет-образец сабмишна (submission.csv.zip)
* [requirements.txt](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/requirements.txt)

### Краткая информация о данных

Исходный данные представляеют собой набор датасетов.

Информация о данных в датасетах:

1. hotels_train.csv.zip 
Первоначальная версия датасета содержит информацию о **386803 записей** (отзывов) по **17 признакам** со следующей информацией:

- hotel_address — адрес отеля;
- review_date — дата, когда рецензент разместил соответствующий отзыв;
- average_score — средний балл отеля, рассчитанный на основе последнего комментария за последний год;
- hotel_name — название отеля;
- reviewer_nationality — страна рецензента;
- negative_review — отрицательный отзыв, который рецензент дал отелю;
- review_total_negative_word_counts — общее количество слов в отрицательном отзыв;
- positive_review — положительный отзыв, который рецензент дал отелю;
- review_total_positive_word_counts — общее количество слов в положительном отзыве.
- reviewer_score — оценка, которую рецензент поставил отелю на основе своего опыта;
- total_number_of_reviews_reviewer_has_given — количество отзывов, которые рецензенты дали в прошлом;
- total_number_of_reviews — общее количество действительных отзывов об отеле;
- tags — теги, которые рецензент дал отелю;
- days_since_review — количество дней между датой проверки и датой очистки;
- additional_number_of_scoring — есть также некоторые гости, которые просто поставили оценку сервису, но не оставили отзыв. Это число указывает, сколько там действительных оценок без проверки.
- lat — географическая широта отеля;
- lng — географическая долгота отеля.

2. hotels_test.csv.zip [Здесь](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model/data)
Первоначальная версия датасета содержит информацию о **128935 записей** (отзывов) по **16 признакам** (без  'reviewer_score').

3. submission.csv.zip [Здесь](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model/data)
Содержит датасет, включающий 128935 строки и два признака 'reviewer_score' и 'id'.


:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Этапы работы над проектом

Выполнение проекта проходило в несколько этапов:

* 1 этап. Отбор необходимых библиотек

- Библиотеки для работы с данными: numpy, pandas;
- Библиотеки для работы с признаками: category_encoders, sklearn (preprocessing);
- Библиотеки  для визуализации: matplotlib.pyplot,  seaborn;
- Библиотеки для оценки тональности текста: nltk (SentimentIntensityAnalyzer)
- Для разделения датасета и работы с моделью:
sklearn.model_selection, sklearn.ensemble (RandomForestRegressor), sklearn (metrics)

* 2 этап. Знакомство с исходными данными

- Первоначальная версия тренировочного датасета содержит информацию о 386803 записях (отзывов) по 17 признакам:
Признаки можно разделить на три группы:

1. Связанные с отелем признаки / Hotel Related Features (7)

- hotel_name - full hotel name;
- hotel_address - address: street, post code, city, country;
- lat - hotel latitude coordinate;
- lng - hotel longitude coordinate;
- average_score - average hotel rating;
- total_number_of_reviews - total number of hotel reviews;
- additional_number_of_scoring - number of hotel scores without review.

2. Связанные с рецензентом признаки / Reviewer Related Features (3)

- reviewer_nationality - reviewer nationality;
- total_number_of_reviews_reviewer_has_given - total number of reviews reviewer has given;
- tags - tags describing stay in the hotel.

3. Связанные с отзывом признаки / Review Related Features (6)

- review_date date of review;
- days_since_review difference in the number of days between review date and scrape date;
- negative_review text of negative review;
- review_total_negative_word_counts negative review words number;
- positive_review text of positive review;
- review_total_positive_word_counts positive review words number.

**Проблемы:**
- Отсутствуют некоторые значения в столбцах lat и lng. 
​
- Числовые значения в 9 столбцах: 'additional_number_of_scoring', 'average_score','review_total_negative_word_counts','total_number_of_reviews_reviewer_has_given', 'total_number_of_reviews',  'review_total_positive_word_counts', 'reviewer_scoretotal_number_of_reviews_reviewer_has_given', 'lat', 'lng'.
​
- Значения типа object в 8 столбцах: 'hotel_address', 'review_date', 'hotel_name', 'reviewer_nationality', 'negative_review', 'positive_review', ' tags ', 'days_since_review'. 


Первоначальная версия тестового датасета содержит информацию о **128935 записей** (отзывов) по **16 признакам** (без  'reviewer_score'). С теми же самыми особенностими и "проблемами".

Первоначальный сабмишн содержит датасет, включающий 128935 строки и два признака 'reviewer_score (пустые значения, нуждается в предсказании) и 'id'

*  3  этап. Подготовка данных, которые будут использованы для обучения модели;

Объединили тестовую и трейн выборки в один датасет и образовав "сигнальный" признак 'sample'.

- Удалили пропущенные значения в признаках 'lat' и 'lng', заменив их на 0.

- Преобразовали некоторые из признаков типа object.
 Признак 'review_date' позволил сгенерировать два новых признака 'day_of_year' (номер дня написания отзыва в году) и 'rewiew_year' (год написания отзыва).

 Из признака 'days_since_review' вычленили числовое значение и перевели в тип int.

 Из признака 'tags' вычленили количество дней пребывания и перевели в тип int, заменив отсутствующие значения на медиану; подсчитали количество слов в тегах.

 Из признака 'negative_review text of negative review' создали бинарный признак 'no_negative', указывающий на информацию нет негатива.

 Из признака 'positive_review text of negative review' создали бинарный признак 'no_positive', указывающий на информацию нет позитива.

 Из обоих признаков 'negative_review text of negative review' и 'positive_review text of negative review' с помощью SentimentIntensityAnalyzer() выделили по четыре характеристики эмоциональной окраски, для которых создали соответствующие признаки: 'negative_neg', 'negative_neu', 'negative_pos', 'negative_compound', 'positive_neg', 'positive_neu', 'positive_pos', 'positive_compound'.

 Из признака 'hotel_address' выделили признак 'city_name': 'London', 'Paris', 'Amsterdam', 'Milan', 'Vienna', 'Barcelona', к которомы применили кодирование One-Hot-Coding, получив пять новых бинарных признаков. Данная информация позволила в признаках 'lat' и 'lng' заменить на координаты города пребывания. Из этого же признака в последствии выделили признак 'country' страна в которой расположен отель.

 К признаку 'hotel_name' применили бинарное кодирование.

 Сравнивая признаки 'country' и 'reviewer_nationality' создали новый бинарный признак 'local_reviewer', указывающий, что гость - "внутренний" путешественник. Сам признак 'reviewer_nationality' подвергли бинарному кодированию.
 
 Итоговый датасет содержал 515738 строк и 48 (+31 новых числовых) признаков.

*  4 этап. Отбор признаков

 Оценили степень мультиколлениарности полученных числовых признаков. Отмечалась высокая корреляция между признаками 'days_since_review' - 'rewiew_year'(-0.92), 'negative_neg' - 'negative_neu' (-0.94), 'negative_neg' - 'no_negative' (0,95), 'negative_neu' - 'no_negative' (0,9),   'positive_pos'  - 'positive_neu'(-0.92) и 'positive_neg' - 'no_positive' (0,91).

 Методом проб наиболее высокая степень точности модели наблюдалась при удалении признаков 'rewiew_year' и 'no_negative'.
 Также удалили оставшиеся признаки типа "object" и "datatime".

*  5 этап. Создание и обучение модели;

 Подготовили обучающую и тестовые выборки. Воспользовались специальной функцией train_test_split для разбивки тестовых данных (20% данных на валидацию): 386485 и 128935 записей соответственно.

 Создали и обучили регрессивную модели by RandomForestRegressor

*  6 этап. Оценка эффективности модели;

 В качестве статистической меры использовалась **MAPE (Mean Absolute Percentages Error).**. Он составил 12.54 %.

*   7 этап. Предсказание моделью результатов по тестовым данным;
 
 Произвели предсказание рейтинга отелий по тестовым данным.

*  8 этап. Подготовка сабмишна;

 Полученные значения перенесли в сабмишин и записали в файл submission.csv

*  9 этап. Отправка результатов на соревнование в Kaggle

 Результаты работы модели (файл submission.csv) отправидли для участия в соотвествующее соревновании на [Kaggle](https://www.kaggle.com/code/ekaterinaarsa/booking-model?scriptVersionId=125799483)
 

*  10 этап. Подготовка и выгрузка проекта в GitHub.

 Оформление проекта производилось на локальном компьютере, созданы вспомогательные файлы requirements.txt, README.md.


:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Предварительные выводы

 На основе проведенного анализа и преобразования исходных данных удалось обучить модель демонстрирующую точность 12.54 % по заданной статистическрой мере MAPE (Mean Absolute Percentages Error).

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Используемые зависимости
отражены в приложенном файле requrments.txt [Здесь](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/requirements.txt))

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Установка проекта

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model
```
:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Использование проекта
Вся информация о проделанной работе представлена в jupyter-ноутбуке [booking_model.ipynb](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/booking_model.ipynb)

## Авторы

* Арсентьева Екатерина Владимировна 

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Результаты
 
 Проведенный анализ и преобразование исходных позволил создать модель, демонстрирующую достаточно высокую точность - 12.54 % по заданной статистическрой мере MAPE (Mean Absolute Percentages Error).

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)


# <center> Exploratory data analysis and building a regression model that predicts the rating of hotels </center> [К русской версии](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#-%D1%80%D0%B0%D0%B7%D0%B2%D0%B5%D0%B4%D1%8B%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B9-%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85-%D0%B8-%D0%BF%D0%BE%D1%81%D1%82%D1%80%D0%BE%D0%B5%D0%BD%D0%B8%D0%B5-%D1%80%D0%B5%D0%B3%D1%80%D0%B5%D1%81%D1%81%D0%B8%D0%B2%D0%BD%D0%BE%D0%B9-%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8-%D0%BF%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D1%8B%D0%B2%D0%B0%D1%8E%D1%89%D0%B5%D0%B9-%D1%80%D0%B5%D0%B9%D1%82%D0%B8%D0%BD%D0%B3-%D0%BE%D1%82%D0%B5%D0%BB%D0%B5%D0%B9--english-version)

## Table of contents

1. [Project description](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#project-description)

1.1. [Brief information about the data](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#brief-information-about-the-data)

1.2. [Stages of work on the project](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/README.md#stages-of-work-on-the-project)
    
1.3. [Preliminary conclusions](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#preliminary-conclusions)

2. [Used libraries](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#used-libraries)

3. [Project uploading](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#project-uploading)

4. [Application of project](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#application-of-project)

5. [Autors](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#autors)

6. [Results](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#results)

## Project description

**This project** is aimed at studying the structure and dependencies (intelligence analysis) of data, selecting and transforming features for training a model that predicts the rating of hotels, based on datasets of 515,000 reviews of hotels in Europe according to the Booking website. **MAPE was used as a statistical measure. (Mean Absolute Percentages Error)**.

# Task:
Based on the dataset of 515,000 hotel reviews in Europe, train a model that should predict the rating of a hotel according to the Booking website.

## Problem:
The presence of hotels winding up their rating on Booking

## Objective of the project:
Build a model based on machine learning algorithms that predicts the rating of a hotel.


Our project includes several stages:

- selection of necessary libraries;
- familiarity with the source data;
- preparation of data that will be used to train the model;
- feature selection;
- creation and training of the model;
- evaluation of the effectiveness of the model;
- model prediction of results from test data;
- Submission preparation;
- sending results to the competition in Kaggle;
- drawing conclusions and uploading to GitHub.


** Structure of project:**
[submission](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/submission.csv)
* [Notebook with code/Booking_model.ipynb](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/booking_model.ipynb)
* [Data folder](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model/data) test dataset (hotels_test.csv.zip) and submission sample dataset (submission.csv.zip).
* [requirements.txt](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/requirements.txt)

### Brief information about the data

TThe initial data is a set of datasets.

Information about data in datasets:

1. hotels_train.csv.zip
The initial version of the dataset contains information about **386803 records** (reviews) for **17 features** with the following information:

- hotel_address — hotel address;
- review_date — the date when the reviewer posted the corresponding review;
- average_score - the average score of the hotel, calculated on the basis of the last comment for the last year;
- hotel_name — hotel name;
- reviewer_nationality — reviewer's country;
- negative_review - negative review given by the reviewer to the hotel;
- review_total_negative_word_counts - total number of words in the negative review;
- positive_review — positive review given by the reviewer to the hotel;
- review_total_positive_word_counts - total number of words in a positive review.
- reviewer_score — rating given by the reviewer to the hotel based on their experience;
- total_number_of_reviews_reviewer_has_given - the number of reviews that reviewers have given in the past;
- total_number_of_reviews - the total number of valid hotel reviews;
- tags — tags that the reviewer gave to the hotel;
- days_since_review - number of days between the review date and the cleanup date;
- additional_number_of_scoring - there are also some guests who simply rated the service, but did not leave a review. This number indicates how many valid grades there are without validation.
- lat - geographical latitude of the hotel;
- lng — geographic longitude of the hotel.

2. hotels_test.csv.zip [Here](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model/data)
The initial version of the dataset contains information about **128935 records** (reviews) for **16 features** (without 'reviewer_score').

3. submission.csv.zip [Here](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model/data)
Contains a dataset containing 128935 rows and two features 'reviewer_score' and 'id'.

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)

### Stages of work on the project

The project was carried out in several stages:

* Stage 1. Selecting the required libraries

  - Libraries for working with data: numpy, pandas;
 - Libraries for working with features: category_encoders, sklearn (preprocessing);
 - Libraries for visualization: matplotlib.pyplot, seaborn;
 - Libraries for evaluating the sentiment of the text: nltk (SentimentIntensityAnalyzer)
 - To separate the dataset and work with the model:
sklearn.model_selection, sklearn.ensemble(RandomForestRegressor), sklearn(metrics)

* Stage 2. Getting to Know the Source Data

 - The initial version of the training dataset contains information about 386803 records (reviews) for 17 features:
Signs can be divided into three groups:

 1. Hotel Related Features (7)

  - hotel_name - full hotel name;
  - hotel_address - address: street, post code, city, country;
  - lat - hotel latitude coordinate;
  - lng - hotel longitude coordinate;
  - average_score - average hotel rating;
  - total_number_of_reviews - total number of hotel reviews;
  - additional_number_of_scoring - number of hotel scores without review.

 2. Reviewer Related Features (3)

  - reviewer_nationality - reviewer nationality;
  - total_number_of_reviews_reviewer_has_given - total number of reviews reviewer has given;
  - tags - tags describing stay in the hotel.

 3. Review Related Features (6)

  - review_date date of review;
  - days_since_review difference in the number of days between review date and scrape date;
  - negative_review text of negative review;
  - review_total_negative_word_counts negative review words number;
  - positive_review text of positive review;
  - review_total_positive_word_counts positive review words number.

**Problems:**

 - Some values are missing in the 'lat' and 'lng' columns.

 - Values of type numeric in 9 columns:'additional_number_of_scoring', 'average_score','review_total_negative_word_counts','total_number_of_reviews_reviewer_has_given', 'total_number_of_reviews',  'review_total_positive_word_counts', 'reviewer_scoretotal_number_of_reviews_reviewer_has_given', 'lat', 'lng'.

 - Values of type object in 8 columns: 'hotel_address', 'review_date', 'hotel_name', 'reviewer_nationality', 'negative_review', 'positive_review', ' tags ', 'days_since_review'.


- The initial version of the test dataset contains information about **128935 records** (reviews) for **16 features** (without 'reviewer_score'). With the same features and "problems".

- The initial submission contains a dataset containing 128935 rows and two features 'reviewer_score (empty values, needs to be predicted) and 'id'

* Stage 3. Preparing the data that will be used to train the model;

We combined the test and train samples into one dataset and formed the "signal" feature 'sample'.

- Removed missing values in the features 'lat' and 'lng', replacing them with 0.

- Converted some of the features of the object type.
  The 'review_date' feature allowed us to generate two new features 'day_of_year' (the day the review was written in a year) and 'review_year' (the year the review was written).

  A numeric value was extracted from the 'days_since_review' feature and converted to the int type.

  The number of days of stay was isolated from the feature 'tags' and transferred to the int type, replacing the missing values with the median; counted the number of words in the tags.

 From the feature 'negative_review text of negative review', a binary feature 'no_negative' was created, indicating that there is no negative information.

  From the feature 'positive_review text of negative review', a binary feature 'no_positive' was created, indicating that there is no positive information.

  From both features 'negative_review text of negative review' and 'positive_review text of negative review', using SentimentIntensityAnalyzer(), four characteristics of emotional coloring were identified, for which the corresponding features were created: 'negative_neg', 'negative_neu', 'negative_pos', 'negative_compound ', 'positive_neg', 'positive_neu', 'positive_pos', 'positive_compound'.

  From the feature 'hotel_address', the feature 'city_name' was extracted: 'London', 'Paris', 'Amsterdam', 'Milan', 'Vienna', 'Barcelona', to which we applied One-Hot-Coding, obtaining five new binary features . This information made it possible to replace 'lat' and 'lng' with the coordinates of the host city. Later, the 'country' attribute, the country in which the hotel is located, was isolated from the same attribute.

  The feature 'hotel_name' has been binary coded.

Comparing the traits 'country' and 'reviewer_nationality' created a new binary trait 'local_reviewer' indicating that the guest is a "domestic" traveler. The feature itself 'reviewer_nationality' was subjected to binary encoding.
 
  The final dataset contained 515738 rows and 48 (+31 new numeric) features.

* Stage 4. feature selection

  The degree of multicolleniality of the obtained numerical features was estimated. There was a high correlation between the features 'days_since_review' - 'rewiew_year' (-0.92), 'negative_neg' - 'negative_neu' (-0.94), 'negative_neg' - 'no_negative' (0.95), 'negative_neu' - 'no_negative' ( 0.9), 'positive_pos' - 'positive_neu'(-0.92) and 'positive_neg' - 'no_positive' (0.91).

  By trial method, the highest degree of model accuracy was observed when the features 'rewiew_year' and 'no_negative' were removed.
  We also removed the remaining features of the "object" type.

* Stage 5. Model creation and training;

  Prepared training and test sets. We used the special function train_test_split to split the test data (20% of the data for validation): 386485 and 128935 records, respectively.

  Created and trained a regression model by RandomForestRegressor

* Stage 6. Evaluation of the effectiveness of the model;

  **MAPE (Mean Absolute Percentages Error) was used as a statistical measure.**. It amounted to 12.54%.

* Stage 7. Model prediction of results from test data;
 
  We made a prediction of the rating of hotels according to test data.

* Stage 8. Submission preparation;

  The received values were transferred to the submission and written to the submission.csv file

* Stage 9. Submitting results to a competition in [Kaggle](https://www.kaggle.com/code/ekaterinaarsa/booking-model?scriptVersionId=125799483)

  The results of the model (file submission.csv) were sent to participate in the appropriate competition on Kaggle.

* Stage 10. Drawing conclusions and uploading to GitHub.

 The design of the project was carried out on the local computer, auxiliary files requirements.txt, README.md were created.


:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)

### Preliminary conclusions

  Based on the analysis and transformation of the initial data, it was possible to train the model with an accuracy of 12.54% for a given statistical measure MAPE (Mean Absolute Percentages Error).


:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)

## Used libraries

reflected in the attached file requrments.txt [Here](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/requirements.txt)

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)

## Project uploading

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model
```

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)

## Application of project
Total information (code) about the work is presented in the jupyter notebook [booking_model.ipynb](https://github.com/EkaterinaArsa/DS_projects/blob/master/Booking_model/booking_model.ipynb)

## Autors

* Arsenteva Ekaterina

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)

## Results
 
  The performed analysis and transformation of the initial ones made it possible to create a model that demonstrates a fairly high accuracy - 12.54% for a given statistical measure MAPE (Mean Absolute Percentages Error).

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/Booking_model#table-of-contents)
