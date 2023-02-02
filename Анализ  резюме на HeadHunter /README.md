
![](./images/data_cleaning.png)
# <center> Очистка данных на Python </center>

# <center> Data cleaning by Python </center>
[English version]()

## Оглавление
1. [Описание проекта](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

1.1. [Краткая информация о данных](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%B0%D1%8F-%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)

1.2. [Этапы работы над проектом](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)
    
1.3. [Результаты и предварительные выводы](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B-%D0%B8-%D0%BF%D1%80%D0%B5%D0%B4%D0%B2%D0%B0%D1%80%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

2. [Используемый зависимости](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D1%8B%D0%B5-%D0%B7%D0%B0%D0%B2%D0%B8%D1%81%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8)

3. [Установка проекта](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

4. [Использование проекта](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

5. [Авторы](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B0%D0%B2%D1%82%D0%BE%D1%80%D1%8B)

6. [Выводы](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

## Описание проекта

**Данный проект** направлен на исследование структуры, преобразование, исследование зависимостей (разведывательный анализ) и очистку данных,  представленных в резюме на HeadHunter


** О структуре проекта:**
* [data](./) - папка с исходными табличными данными (zip и csv форматы)
* [pictures](./pictures) - папка с изображениями, необходимыми для проекта
* [Analysis_of_HeadHunter_info.ipynb](./Analysis_of_HeadHunter_info.ipynb)  - jupyter-ноутбук, содержащий основной код проекта, в котором демонстрируются методы и подходы решения задач очистки данных. Из-за ограничений на размер файлов загружаемых на/с GitHub файл не содержит результатов выполнения кода. Интерактивные графики можно увидеть  [Ссылка на код в Google colab со всеми графиками](https://colab.research.google.com/drive/1STPIT1_R1Y9E8DT_4IveQQPKc-bI6VRf?usp=sharing)
[Ссылка на код в NBViewer со всеми графиками](https://nbviewer.org/github/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/Analysis_of_HeadHunter_info.ipynb)

### Краткая информация о данных

В этом проекте используются данные 44744 резюме [источник: HeadHunter] от hh.ru. Файл с данными можно найти [Google диск](https://drive.google.com/drive/folders/1FLa3snx4lB-bvqdkVEidA4PnRNz0rTSD).[GitHub](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/data)

Необходимо было провести разведывательный анализ и первичную очистку данных, с целью будущего  построения модели, которая бы прогнозировала размеры заработной платы предлагаемой соискателям, опираясь на параметры самого соискателя, и его особенности.

Исходный датасет представляет собой набор данных из таблицы с информацией о параметрах соискателя в резюме, а также таблицы, в которой содержится информация о курсах валют на момент написания/обновления резюме. 

Используемый для анализа датасет содержит информацию из 44744 резюме по 12 признакам, описывающих жилье. Файл с данными резюме можно найти [Google диск](https://drive.google.com/file/d/1zrR8KfEBmlOZFxUMceqhThCVZIbDmhun/view?usp=share_link) [GitHub](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/data). Файл с данными по курсу валют можно найти [Google диск]](https://drive.google.com/file/d/1zrR8KfEBmlOZFxUMceqhThCVZIbDmhun/view?usp=share_link) [GitHub](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/data).

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/ca1c53659e2b5e48c92419a574247bc2b5af2b9a/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Этапы работы над проектом

Выполнение проекта проходило в 5 этапа:

* 1 этап. Исследование структуры данных

Включал в себя знакомство с датасетом, его признаками и основными статистическим данными.

* 2 этап. Преобразование данных

Включало в себя трансформацию неинформативных признаков в информативные. 
* Путем выделения важных признаков из множества. Например: Признак "Город, переезд, командировки" был преобразован в три отдельных информативных признака **"Город"**, **"Готовность к переезду"**, **"Готовность к командировкам"**, имеющим вероятное влияние на уровень предполагаемой заработной платы.
* Также данные приводились к общему показателю. Например: признак "ЗП", изначально указанный в различных видах валюты, трансформировали в признак **"ЗП (руб)"**, в котором зарплата отражалась в рублях.
* Уменьшали количество уникальных значений. Например: город пребывания соискателя был соотнесен с одной из 4 категорий: "Москва", "Санкт-Петербург" и "город-миллионник", остальные обозначьте как "другие".
* Некоторые категориальных признаков преобразовали методом One Hot Encoding.

* 3 этап. Исследование зависимостей данных

Для исследования зависимостей  применяли метод визуализации. Для визуализации в проекте преимущественно использованы plotly.graph_objects, plotly.express, matplotlib.pyplot и seaborn.

Интерактивные графики можно увидеть  [Ссылка на код в Google colab со всеми графиками](https://colab.research.google.com/drive/1STPIT1_R1Y9E8DT_4IveQQPKc-bI6VRf?usp=sharing) 
[Ссылка на код в NBViewer со всеми графиками](https://nbviewer.org/github/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/Analysis_of_HeadHunter_info.ipynb)

* 4 этап. Очистка данных

> **Очистка данных (data cleaning)** – это процесс обнаружения и удаления (или исправления) поврежденных, ложных или неинформативных записей таблицы или целой базы данных. Процесс состоит из двух этапов: поиск и ликвидация (или редактирование).

Основные этапы очистки данных:
* Работа с пропущенными значениями.
* Очистка данных от пропусков.
* Удаление признаков и записей, которые не несут полезной информации, в том числе выбросы.

**Цель очистки данных** — избавиться от «мусора», который может помешать моделированию или исказить его результаты. Во многих задачах очистка данных — это самая главная часть этапа подготовки данных к построению модели, которая нередко занимает большую часть времени работы над задачей.
ng)

* 5 этап. Подготовка документации, выгрузка датасетов на Google-диск, а также других файлов в GitHub

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Результаты и предварительные выводы

* Большая часть соискателей в возрасте 27-36 лет
* Большая часть соискателей имеет опыт 57-154 месяца.
* Большая часть соискателей рассчитывает на зарплату 40-100 тысяч 
* Отмечается прямая зависимость желаемой заработной платы от уровня образования соискателяю Наибольшую заработную плату желают получить соискатели, имеющие высшее образование.
* Наибольшую заработную плату желают получить соискатели, проживающие в Москве и Санкт-Петербурге.
* Готовность как к переезду, так и к командировкам способствует более высоким требованиям к желаемой заработной плате. Неготовность ездить в командировки сильно снижает уровень притязаний.
* Среди лиц с высшим  образованием в большинстве своем наблюдается возрастание (самое быстрое из всех групп) уровня желаемой зарплаты к 40 годам (38-45 лет).
* Готовность к переезду и командировкам у мужчин выше, чем у женщин, и независимо от пола готовность к переезду несколько повышается в возрасте старше 20 лет (до 48 лет у мужчин, до 34 лет у женщин). Следует отметить скачок готовности поехать в 60 и 70 лет. Мужчины демонстрируют высокую готовность к командировкам независимо от возраста (наибольшую до 60 лет).
* Средний уровень желаемой зарплаты у мужчин выше, чем у женщин.

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Используемые зависимости
* Python (3.9):
    * [numpy (1.23.4)](https://numpy.org)
    * [pandas (1.5.2)](https://pandas.pydata.org)
    * [matplotlib (3.6.2)](https://matplotlib.org)
    * [plotly(5.11.0) модули  plotly.express и plotly.offline](https://plotly.com/)
    * [seaborn(0.12.1)](https://seaborn.pydata.org/)

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Установка проекта

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20
```
:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Использование проекта
Вся информация о работе представлена в jupyter-ноутбуке Analysis_of_HeadHunter_info.ipynb.

## Авторы

* Арсентьева Екатерина Владимировна 

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Выводы

Данный проект выявил ряд признаков, позволяющих прогнозировать вероятную заработную плату, которую можно предложить соискателю с учетом его особенностей. Так уровень заработной платы напрямую зависит от места проживания соискателя (крупные города), уровню образования, опыту работы, готовности к переезду и командировкам. Также следует отметить, что более высокий уровень предполагаемой заработной платы имеют лица среднего возраста, мужского пола, но в данном случае нельзя исключать связь с большей мобильностью данной группы соискателей (готовностью к перезду и командировкам).

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)


## English Version

## Table of contents

1. [Project description](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

1.1. [Brief information about the data](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%B0%D1%8F-%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)

1.2. [Stages of work on the project](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)
    
1.3. [Results and preliminary conclusions](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B-%D0%B8-%D0%BF%D1%80%D0%B5%D0%B4%D0%B2%D0%B0%D1%80%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

2. [Used libraries](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D1%8B%D0%B5-%D0%B7%D0%B0%D0%B2%D0%B8%D1%81%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8)

3. [Project uploading](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

4. [Application of project](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

5. [Autors](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B0%D0%B2%D1%82%D0%BE%D1%80%D1%8B)

6. [Conclusions](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

## Project description

**This project** aims to study the structure, transformation of data, study of its dependencies and clean up it presented in the summary on HeadHunter


** Structure of project:**
* [data](./) - filefolder with initial tabular data (zip and csv formats)
* [pictures](./pictures) - filefolder with images needed for the project
* [Analysis_of_HeadHunter_info.ipynb](./Analysis_of_HeadHunter_info.ipynb)  - jupyter-ноутбук, containing the main code of the project, which demonstrates methods and approaches for solving data cleaning problems. Due to size restrictions on uploading files to/from GitHub, the file does not contain the results of code execution. Interactive charts can be seen  [Link to Google colab includes plots](https://colab.research.google.com/drive/1STPIT1_R1Y9E8DT_4IveQQPKc-bI6VRf?usp=sharing)
[Link to NBViewer includes plots](https://nbviewer.org/github/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/Analysis_of_HeadHunter_info.ipynb)

### Brief information about the data

This project uses data from 44744 resumes [source: HeadHunter] from hh.ru. The data file can be found [Google диск](https://drive.google.com/drive/folders/1FLa3snx4lB-bvqdkVEidA4PnRNz0rTSD).[GitHub](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/data)

It was necessary to conduct an exploratory analysis and primary data cleaning, with the aim of building a future model that would predict the amount of wages offered to job seekers, based on the parameters of the job seeker and his characteristics.

The initial dataset is a data set from a table with information about the parameters of the applicant in the resume, as well as a table that contains information about exchange rates at the time of writing/updating the resume.

The dataset used for the analysis contains information from 44744 abstracts for 12 features describing housing. Resume file can be found [Google диск](https://drive.google.com/file/d/1zrR8KfEBmlOZFxUMceqhThCVZIbDmhun/view?usp=share_link) [GitHub](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/data). Файл с данными по курсу валют можно найти [Google диск]](https://drive.google.com/file/d/1zrR8KfEBmlOZFxUMceqhThCVZIbDmhun/view?usp=share_link) [GitHub](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/data).

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/blob/ca1c53659e2b5e48c92419a574247bc2b5af2b9a/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Stages of work on the project

Выполнение проекта проходило в 5 этапа:

The project was carried out in 5 stages:

* Stage 1. Data structure research

It included an acquaintance with the dataset, its features and basic statistical data.

* Stage 2. Data conversion

It included the transformation of non-informative features into informative ones.
* By highlighting important features from the set. For example: The attribute "Городб готовность к перезду и командировкам" ("City, moving, business trips") was converted into three separate informative attributes **"Город"** ("City"), **Готовность к переезду** ("Ready to move/change city"), **Готовность к командировкам"** ("Ready to bisness traveling"), having a likely impact on the level expected salary.
* Also, the data were given to the general indicator. For example: the feature "ЗП" (salary), originally indicated in various types of currency, was transformed into the feature **"ЗП (руб)"** (salary in rubles), in which the salary was reflected in rubles.
* Reduced the number of unique values. For example: the applicant's city of residence was assigned to one of 4 categories: "Москва" ("Moscow"), "Санкт-Питербург" ("St. Petersburg") and "Города-миллионники" ("million population city"), designate the rest as "другие" "other".
* Some categorical features were converted using the One Hot Encoding method.

Stage 3. Exploring data dependencies

The visualization method was used to study dependencies. For visualization, the project mainly used plotly.graph_objects, plotly.express, matplotlib.pyplot и seaborn.

Interactive plots are presented [Link to Google colab includes plots](https://colab.research.google.com/drive/1STPIT1_R1Y9E8DT_4IveQQPKc-bI6VRf?usp=sharing)
[Link to NBViewer includes plots](https://nbviewer.org/github/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/Analysis_of_HeadHunter_info.ipynb)

* Stage 4. Data cleansing

> **Data cleaning** is the process of detecting and removing (or fixing) corrupted, false, or uninformative features in a table or entire database. The process consists of two stages: search and liquidation (or editing).

The main stages of data cleaning:
* Dealing with missing values.
* Clearing data from gaps.
* Remove features and entries that не несут полезной информации, o not carry useful information, including outliers.

**The purpose of data cleansing** is to get rid of "garbage" that can interfere with the simulation or distort its results. In many tasks, data cleansing is the most important part of the stage of data preparation for building a model, which often takes up most of the work on a task.

* * Stage 5. Preparation of documentation, uploading datasets to Google Drive, as well as other files to GitHub

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Results and preliminary conclusions

* Most applicants are aged 27-36
* Most applicants have 57-154 months of experience.
* Most applicants expect a salary of 40-100 thousand
* There is a direct dependence of the desired salary on the level of education of the applicant. The highest salary is desired by applicants with higher education.
* Applicants living in Moscow and St. Petersburg wish to receive the highest salary.
* Willingness to both relocate and bisness traveling contributes to higher requirements for desired wages. Unwillingness to go on business trips greatly reduces the level of claims.
* Among people with higher education, for the most part, there is an increase (the fastest of all groups) in the level of the desired salary by the age of 40 (38-45 years).
The willingness to move and business trips among men is higher than among women, and regardless of gender, the willingness to move slightly increases at the age of over 20 years (up to 48 years for men, up to 34 years for women). It should be noted the jump in willingness to travel at 60 and 70 years old. Men demonstrate a high readiness for business trips regardless of age (the highest is up to 60 years).
* The average level of desired salary for men is higher than for women.

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Used libraries
* Python (3.9):
    * [numpy (1.23.4)](https://numpy.org)
    * [pandas (1.5.2)](https://pandas.pydata.org)
    * [matplotlib (3.6.2)](https://matplotlib.org)
    * [plotly(5.11.0) модули  plotly.express и plotly.offline](https://plotly.com/)
    * [seaborn(0.12.1)](https://seaborn.pydata.org/)

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Project uploading

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20
```
:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Use of project
All information (code) is presented in jupyter-ноутбуке Analysis_of_HeadHunter_info.ipynb.

## Autors

* Arsenteva Ekaterina

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Conclusions

This project has identified a number of indicators that allow you to predict the likely salary that can be offered to the applicant, taking into account his characteristics. So the level of wages directly depends on the place of residence of the applicant (large cities), the level of education, work experience, readiness to move and business trips. It should also be noted that middle-aged males have a higher level of expected wages, but in this case, the connection with the greater mobility of this group of applicants (willingness to changing of city and business traveling) cannot be ruled out.

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)