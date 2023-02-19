
![](./images/data_cleaning.png)
# <center> Использование SQL+Python для анализа данных </center>

# <center> Application of SQL+Python for data analysis </center> [English version](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#english-version)

## Оглавление
1. [Описание проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

1.1. [Краткая информация о данных](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%B0%D1%8F-%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)

1.2. [Этапы работы над проектом](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)
    
1.3. [Результаты и предварительные выводы](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B-%D0%B8-%D0%BF%D1%80%D0%B5%D0%B4%D0%B2%D0%B0%D1%80%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

2. [Используемый зависимости](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D1%8B%D0%B5-%D0%B7%D0%B0%D0%B2%D0%B8%D1%81%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8)

3. [Установка проекта](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/README.md#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

4. [Использование проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

5. [Авторы](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D0%B0%D0%B2%D1%82%D0%BE%D1%80%D1%8B)

6. [Выводы](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization#%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

## Описание проекта

**Данный проект** направлен на исследование структуры и зависимостей (разведывательный анализ)  данных,  по вакансиям на HeadHunter, представленных в виде пяти таблиц в METABASE c использованием возможностей SQL


Наш проект включает в себя несколько этапов:

- выбор необходимых библиотек;
- формирование подключения к базе данных;
- предварительный анализ данных и знакомство с ними;
- детальный анализ вакансий;
- анализ работодателей;
- предметный анализ (вакансии для DataScience);
- оформление выводов и загрузка на GitHub.

** О структуре проекта:**

* [Папка с информацией о таблицах](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization/Tables)
* [HHru analysis(sql+python+visualization).ipynb](./Analysis_of_HeadHunter_info.ipynb)  - jupyter-ноутбук,  из-за некоторых особенностей взаимодействия GitHub и библиотеки Plotly файл не содержит некоторых результатов визуализации. Интерактивные графики можно увидеть  
[Ссылка на код в NBViewer со всеми графиками](https://nbviewer.org/github/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/Analysis_of_HeadHunter_info.ipynb)

### Краткая информация о данных

Исходный данные представляеют собой набор таблиц на сайте Metabase с информацией о параметрах соискателя в резюме, а также таблицы, в которой содержится информация о курсах валют на момент написания/обновления резюме. 


Необходимо было провести разведывательный анализ и первичную очистку данных, с целью будущего  построения модели, которая бы прогнозировала размеры заработной платы предлагаемой соискателям, опираясь на параметры самого соискателя, и его особенности.

1. VACANCIES [Здесь]()
Таблица хранит в себе данные по вакансиям.

2. AREAS[Здесь]()
Таблица-справочник, которая хранит код города и его название.

3. EMPLOYERS [Здесь]()
Таблица-справочник со списком работодателей.

4. INDUSTRIES [Здесь]()
Таблица-справочник вариантов сфер деятельности работодателей.

5. EMPLOYERS_INDUSTRIES [Здесь]()
Дополнительная таблица, которая существует для организации связи между работодателями и сферами их деятельности.

Используемые для анализа данные содержат информацию из 49190 резюме, 23501 работодателе и  1362 регионах.

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Этапы работы над проектом

Выполнение проекта проходило в несколько этапов:

* 1 этап. Выбор необходимых библиотек

 - Библиотеки для работы с запросами SQL: pandas, sqlalchemy, psycopg2
 - Библиотеки для визуализации: seaborn, plotly.express, plotly.graph_objects
 - Библиотеки для отображения графиков plotly через сайт nbviewer.org: plotly.offline, plotly.io as pio

* 2 этап. Формирование подключения к базе данных
 
 Для подключения к бозе данных была создана функция **query_func**, которая обеспечивала отправку запроса с помощью sqlalchemy и возврат результата в виде DateFrame.

* 3 этап. Предварительный анализ данных и знакомство с ними

 Включал в себя знакомство с датасетами, его признаками и определены размеры основных датасетов (vacancies, employers, areas, industries).

* 4 этап. Детальный анализ вакансий

 Определялось наличие вакансий по регионам, наличие указаний на уровень зарплаты и ее средние и медианные значения, варианты сочетаний типа рабочего графика и типа трудоустройства, требования к опыту работы. Некоторые из результатов для улучшения восприятия визуализированы в графиках.

* 5 этап. Анализ работодателей

 Определялось количество вакансий по каждому из ракботодателей, в том числе и по регионам, наличие указанной сферы деятельности, отдельно определены работододатели, занимающиеся разработкой програмного обеспечения, и наличие вакансий по наиболее топовому работодателю - Яндекс в городах-миллионниках, данные о которых получили с помощью html-запроса.

* 6 этап. Предметный анализ (вакансии для DataScience);

Определено общее количество вакансий для специалистов, связанных с обработкой данных, сколько из этих вакансий подходит для специалистов в DS уровня Junior, как часто для специалистов в области DS необходимо знание SQL, Poostgres и Python, сколько в среднем ключевых навыков требуется и каков уровень предлагаемой заработной платы для датасайентистов в зависимости от опыта.

* 7 этап. Оформление выводов и загрузка на GitHub.

В каждом блоке представлены выводы, на 7 этапе сделаны заключения о том, какие вопросы возникли при проведении анализа и какие дальнейшие векторы изучения данных выявлены. В качестве демонстрации проведено исследование данных для ответа на некоторые из возникших вопросов (оценка влияния на предполагаемую зарплату уровня опыта и вида рабочего графика; оценка зависимости результата анализа признака заработной платы, уровня требуемого опыта от сферы деятельности, на примере Яндекса по вакансиям в области DS).


Интерактивные графики можно увидеть  [Ссылка на код в NBViewer со всеми графиками](https://nbviewer.org/github/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20/Analysis_of_HeadHunter_info.ipynb)

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

### Результаты и предварительные выводы

**Выводы по предварительному анализу данных:**
 - В представленной нам схеме (public) в базе данных (project_sql) 5 таблиц: vacancies, employers, areas, industries и employers_industries. В них   представлены данные по 49197 вакансиям(согласно таблице vacancies), 23501 работодателям (согласно таблице employers), 1362 регионам (городам) (согласно таблице areas) и 294 сферам деятельности (согласно таблице industries). Таблица employers_industries вспомогательная и демонстрирует связь между работодателями и сферами их деятельности.

**Выводы по детальному анализу вакансий:**
 - Наибольшее количество вакансий приходится на  крупные города. В . ТОП-5 вошли: по России: Москва - 5333 вакансии, Санкт-Питербург - 2851 вакансия, Новосибирск - 2006 вакансий; по СНГ Минск - 2112 вакансий, Алма-Аты - 1892 вакансии.

 - Более, чем в половине случаев (24073 из 49197), в вакансиях указан минимальный и/или максимальный уровень предполагаемой заработной платы.

 - Средние значения "зарплатной вилки" находятся в интервале от 71065 до 110537. Но учитывая большое количество вакансий с неуказанными уровнями предполагаемой зарплаты, данные цифры нуждаются в дальнейшей корректировке и изучении. Кроме того, по данному признаку, вероятно, имеются множественные выбросы.

 - Большая часть вакансий предусматривает полный рабочий день и полную занятость (35367 вакансий), меньше предлагают удаленную работу при полной занятости (7802 вакансии). Вахтовый тип рабочего графика не предлагается при стажировке и частичной занятости. !Интересно посмотреть, как тип грабочего графика и занятости связан с требуемым опытом и влияет на зарплату!.

 - Требуемый опыт работы преимущественно в интервале 1-3 года (53.2%, 26152 вакансии), реже - 3-6 лет (29.5%, 14511 вакансий). Без опыта работы соискателей готовы принять в 7197 случаев (14.6%), в 1337 вакансиях требуется опыт работы более 6 лет (2.72%).

**Выводы по результатам анализа работодателей:** 

 - Анализ данных по работодателям показал, что по количеству вакансий в ТОП-5 входят такие "гиганты", как Яндекс (1933 вакансии), Ростелеком (491 вакансия), Тинькофф (444 вакансии), Сбер (428 вакансий) и Газпромнефть (331 вакансия). Что может демонстрировать как активный рост этих компаний, так и высокую "текучку" кадров в них. Так у компании Яндекс имеются вакансии и в 16 городах-миллионниках: Москва, Санкт-Петербург, Екатеринбург,Нижний Новгород, Новосибирск, Воронеж, Краснодар, Самара, Уфа, Казань, Пермь, Ростов-на-Дону, Волгоград, Красноярск, Челябинск, Омск (в порядке убывания количества вакансий);

 - Анализ данных по работодателям показал, что по количеству вакансий в ТОП-5 входят такие "гиганты", как Яндекс (1933 вакансии), Ростелеком (491 вакансия), Тинькофф (444 вакансии), Сбер (428 вакансий) и Газпромнефть (331 вакансия). Что может демонстрировать как активный рост этих компаний, так и высокую "текучку" кадров в них. Так у компании Яндекс имеются вакансии и в 16 городах-миллионниках, рынок трудоустройства в которых обычно достаточно насыщен;

 - По России большинство работодателей, неимеющих вакансий, сосредоточено в Московской области (75 компаний), Краснодарском Крае (19 компаний) и, неожиданно,  в Ростовской области (18 компаний). Что показывает высокую степень насыщения рабочих мест кадрами в этих регионах;

 - Среди компаний, имеющих вакансии в различных регионах, значительно выделяются Яндекс (в 181 регионе имеются вакансии) и Ростелеком (вакансии в 153 регионах), что , вероятно, связано с активным ростом этих компаний-гигантов и постоянной текучкой кадров, а также (!НУЖНО УТОЧНИТЬ!) возможностью удаленной работы. Неожиданно, в пятерку вошли: такая компания как Спецремонт, за счет своей обширности (116 регионов с вакансиями), а также малоизвестные ИП "Поляков Денис Иванович" (за счет дистанционной формы работы по обработке телефонных номеров и массовым недовольством сотрудников уровнем заработной платы) (вакансии в 88 регионах) и ООО ЕФИН (за счет обширной сети филиалов более, чем в 500 городах и массовым недовольством сотрудников организацией трудового процесса и оплаты труда) (вакансии в 71 регионе);

 - В представленных данных у 8419 работодателей (35.8%) нет информации о сфере деятельности, что, вероятно, может затруднить принятие решения об отклике на вакансию среди соискателей. В то же время, у многих компаний представлена информация о нескольких сферах деятельности;

 - Разработкой програмного обеспечения занимаются 3553 компании (15.1%) из списка работодателей (!было бы интересно оценить, какие сферы деятельности наиболее представлены среди работодателей!), рынок трудоустройства в которых обычно достаточно насыщен;

 - По России большинство работодателей, неимеющих вакансий, сосредоточено в Московской области (75 компаний), Краснодарском Крае (19 компаний) и, неожиданно,  в Ростовской области (18 компаний). Что, вероятно, показывает высокую степень насыщения рабочих мест кадрами в этих регионах. !Было бы интересно посмотреть на соотношение числа вакансий, работодателей по этим регионам!;

 - Среди компаний, имеющих вакансии в различных регионах, значительно выделяются Яндекс (в 181 регионе имеются вакансии) и Ростелеком (вакансии в 153 регионах), что , вероятно, связано с активным ростом этих компаний-гигантов и постоянной текучкой кадров. Неожиданно, в пятерку вошли: така крупная компания как Спецремонт (116 регионов с вакансиями), а также малоизвестные ИП "Поляков Денис Иванович" (за счет дистанционной формы работы по обработке телефонных номеров и массовым недовольством сотрудников уровнем заработной платы) (вакансии в 88 регионах) и ООО ЕФИН (за счет обширной сети филиалов более, чем в 500 городах и массовым недовольством сотрудников организацией трудового процесса и оплаты труда) (вакансии в 71 регионе).

**Выводы по предметному анализу ( вакансии для DataScience):**

 - 1771 вакансия (36% от общего числа вакнсий) имеет отношение к работе с данными;

 - Среди вакансий для датасайентистов  51 (2.9%) подходит для соискателей уровня Junior;

 - В среднем, для датасайентистов требуется владение 6-7 навыками, при этом в 201 (11.3%) - содержатся требования о наличии ключевых навыков в использовании SQL и Postres, а в 351 (19.8%) - владение Python;

 - При этом средний уровень предлагаемой заработной платы для таких специалистов (DS) зависит от опыта: для соискателей без опыта он находится на уровне 74643 рубля, с опытом от 1 до 3 лет - 139675 рублей, при опыте 3-6 лет средняя предполагаемая заработная плата составляет 243115 рублей. В предложенных данных отсутствуют вакансии с требованиями к длительности опыта более 6 лет.

**Выводы по результата дополнительного исследования:**

 - наиболее высокий уровень заработной платы имеют сотрудники с опытом работы более 6 лет и работающие вахтовым методом. Удивительно, что для сотрудников с опытом более 6 лет и вахтовым методом уровень заработной платы значительно ниже, чем при опыте менее 6 лет. Вероятно, имеет место наличие "неоднородных" вакансий. Необходимо четко разделить вакансии по сферам деятельности и затем отдельно для каждой сферы провести сравнительный анализ.

 - В вакансиях от Яндкс в 1475 опыт не требуется, 380 вакансий для специалистов с опытом работы 1-3года, 72 вакансии для соискателей с опытом 3-6 лет, 6 вакансий для специалистов с опытом более 6 лет.

 - Медианная предполагаемая зарплата в компании яндекс зависит от региона. Максимальная - в Москве (51000 рублей), минимальная до 15000 во многих регионах(Курган, Краснодар, Косьтрома и тд).

 - Не отмечена прямая зависимость уровня заработной платы от опыта работы. 
   
   - В компанию Яндекс требуются специалисты в DS, которые имеют опыт от 1 до 3 лет (3 вакансии) и еще более 3-6 лет (6 вакансий). Вакансий для Junior и специалистов с опытом более 6 лет нет. Таким образом, в компании Яндекс достаточно высокие требования к уровню опыта для кандидатов по указанной специальности. Специалисты DS с опытом старше 6 лет вообще отсутствуют в вакансиях (как мы отмечали выше), это связано с тем, что их единицы, они известны в данной области и их приглашают на должность адресно.

   - Заработная плата для специалистов DS в компанию Яндекс не указана, что говорит о ее зависимости от результатов собеседования и о том, что кандидатов привлекает имидж компании, а не установленный уровень зарплаты&

   **Продемонстрированные результаты указывают на значительные отличия для каждой профессиональной сферы и на то что нельзя ориентироваться на обобщенные данные.**

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Используемые зависимости
* Python (3.9):
    * [numpy (1.23.4)](https://numpy.org)
    * [pandas (1.5.2)](https://pandas.pydata.org)
    * [SQLAlchemy (2.0.3)](https://www.sqlalchemy.org/)
    * [psycopg2 (2.9.5)](https://www.psycopg.org/)
    * [plotly(5.11.0) модули  plotly.express и plotly.offline](https://plotly.com/)
    * [seaborn(0.12.1)](https://seaborn.pydata.org/)

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Установка проекта

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20
```
:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Использование проекта
Вся информация о работе представлена в jupyter-ноутбуке HHru_analysis(sql+python+visualization).ipynb].ipynb.

## Авторы

* Арсентьева Екатерина Владимировна 

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Выводы

Данный проект выявил ряд признаков, которые нуждаются в предварительной обработке: 

 - Прежде всего, признаки зарплаты (salary_from, salary_to) таблицы vacancies. В данном признаке имеются множественные пропуски, и явные выбросы;

 - В названиях регионов (name) таблицы areas, имеются записи,  не дающие точной информации (например, в качестве региона указывается "Россия"), что может искажать статистику по регионам;

 - У многих работодателей (таблица industries) не представлены сферы деятельности  (name).

 Также при проведении исследования возник ряд вопросов, нуждающихся в дальнейшем изучении.

:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)


## English Version

## Table of contents

1. [Project description](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#project-description)

1.1. [Brief information about the data](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#brief-information-about-the-data)

1.2. [Stages of work on the project](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#stages-of-work-on-the-project)
    
1.3. [Results and preliminary conclusions](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#results-and-preliminary-conclusions)

2. [Used libraries](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#used-libraries)

3. [Project uploading](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#project-uploading)

4. [Application of project](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#application-of-project)

5. [Autors](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#autors)

6. [Conclusions](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#conclusions)

## Project description

**This project** aims to study the structure and dependencies (intelligence analysis) of data from the vaccancies on HeadHunter, presented in the form of five tables in METABASE using SQL capabilities


Our project includes several stages:

- selection of necessary libraries;
- formation of a connection to the database;
- preliminary data analysis and getting to them;
- detailed analysis of vacancies;
- analysis of employers;
- subject analysis (vacancies for DataScience);
- drawing conclusions and uploading to GitHub.


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

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)

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

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)

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

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)

## Used libraries
* Python (3.9):
    * [numpy (1.23.4)](https://numpy.org)
    * [pandas (1.5.2)](https://pandas.pydata.org)
    * [matplotlib (3.6.2)](https://matplotlib.org)
    * [plotly(5.11.0) модули  plotly.express и plotly.offline](https://plotly.com/)
    * [seaborn(0.12.1)](https://seaborn.pydata.org/)

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)

## Project uploading

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20
```
:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)

## Application of project
All information (code) is presented in jupyter-ноутбуке Analysis_of_HeadHunter_info.ipynb.

## Autors

* Arsenteva Ekaterina

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)

## Conclusions

This project has identified a number of indicators that allow you to predict the likely salary that can be offered to the applicant, taking into account his characteristics. So the level of wages directly depends on the place of residence of the applicant (large cities), the level of education, work experience, readiness to move and business trips. It should also be noted that middle-aged males have a higher level of expected wages, but in this case, the connection with the greater mobility of this group of applicants (willingness to changing of city and business traveling) cannot be ruled out.

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%20%D1%80%D0%B5%D0%B7%D1%8E%D0%BC%D0%B5%20%D0%BD%D0%B0%20HeadHunter%20#table-of-contents)