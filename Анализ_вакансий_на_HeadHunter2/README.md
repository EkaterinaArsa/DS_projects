
![](./images/data_cleaning.png)
# <center> Использование SQL+Python для анализа данных </center> [English version](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#-application-of-sqlpython-for-data-analysis--%D0%BA-%D1%80%D1%83%D1%81%D1%81%D0%BA%D0%BE%D0%B9-%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D0%B8)


## Оглавление
1. [Описание проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

1.1. [Краткая информация о данных](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%B0%D1%8F-%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)

1.2. [Этапы работы над проектом](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython)%2Bvisualization#%D1%8D%D1%82%D0%B0%D0%BF%D1%8B-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-%D0%BD%D0%B0%D0%B4-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%BC)
    
1.3. [Результаты и предварительные выводы](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D1%8B-%D0%B8-%D0%BF%D1%80%D0%B5%D0%B4%D0%B2%D0%B0%D1%80%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

2. [Используемый зависимости](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D0%BC%D1%8B%D0%B5-%D0%B7%D0%B0%D0%B2%D0%B8%D1%81%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8)

3. [Установка проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

4. [Использование проекта](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0)

5. [Авторы](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%B0%D0%B2%D1%82%D0%BE%D1%80%D1%8B)

6. [Выводы](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

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

* [Папка с информацией о таблицах](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables)
* [HHru_analysis_sql_python_visualization.ipynb](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/HHru_analysis_vacancies_sql_python_visualization.ipynb)  - jupyter-ноутбук,  из-за некоторых особенностей взаимодействия GitHub и библиотеки Plotly файл не содержит некоторых результатов визуализации. Интерактивные графики можно увидеть  
[Ссылка на код в NBViewer со всеми графиками](https://nbviewer.org/github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/HHru%20analysis(sql%2Bpython%2Bvisualization).ipynb)

### Краткая информация о данных

Исходный данные представляеют собой набор таблиц на сайте Metabase с информацией о вакансиях (Vacancies), работодателях(Employers), регионах (Areas), сферах деятельности(Industries), информация о работодателях и их сферах деятельности (Employers_industries)

Информация о данных в таблицах:

1. VACANCIES [Здесь](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Vacancies.png)
Таблица хранит в себе данные по вакансиям.

2. AREAS[Здесь](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Areas.png)
Таблица-справочник, которая хранит код города и его название.

3. EMPLOYERS [Здесь](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Employers.png)
Таблица-справочник со списком работодателей.

4. INDUSTRIES [Здесь](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Industries.png)
Таблица-справочник вариантов сфер деятельности работодателей.

5. EMPLOYERS_INDUSTRIES [Здесь](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Employers_industries.png)
Дополнительная таблица, которая существует для организации связи между работодателями и сферами их деятельности.

Используемые для анализа данные содержат информацию из 49190 вакансиях, 23501 работодателе и  1362 регионах.

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


Интерактивные графики можно увидеть  [Ссылка на код в NBViewer со всеми графиками](https://nbviewer.org/github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/HHru%20analysis(sql%2Bpython%2Bvisualization).ipynb)

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
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)
```
:arrow_up:[к оглавлению](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#%D0%BE%D0%B3%D0%BB%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5)

## Использование проекта
Вся информация о работе представлена в jupyter-ноутбуке HHru_analysis(sql+python+visualization).ipynb.

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


# <center> Application of SQL+Python for data analysis </center> [К русской версии](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#-%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-sqlpython-%D0%B4%D0%BB%D1%8F-%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%D0%B0-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85--english-version)

## Table of contents

1. [Project description](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#project-description)

1.1. [Brief information about the data](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#brief-information-about-the-data)

1.2. [Stages of work on the project](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#stages-of-work-on-the-project)
    
1.3. [Results and preliminary conclusions](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#results-and-preliminary-conclusions)

2. [Used libraries](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#used-libraries)

3. [Project uploading](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#project-uploading)

4. [Application of project](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#application-of-project)

5. [Autors](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#autors)

6. [Conclusions](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#conclusions)

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
* [Folder with tables information](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables)

* [HHru_analysis_sql_python_visualization.ipynb](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/HHru_analysis_vacancies_sql_python_visualization.ipynb)  [
[Link to NBViewer includes plots](https://nbviewer.org/github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/HHru%20analysis(sql%2Bpython%2Bvisualization).ipynb)

### Brief information about the data

The initial data is a set of tables on the Metabase website with information about vacancies (Vacancies), employers (Employers), regions (Areas), fields of activity (Industries), information about employers and their fields of activity (Employers_industries)

Information about data in tables:

1. VACANCIES [Here](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Vacancies.png)
The table contains data on vacancies.

2. AREAS[Here](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Areas.png)
Reference table that stores the city code and its name.

3. EMPLOYERS [Here](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Employers.png)
Reference table with a list of employers.

4. INDUSTRIES [Here](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Industries.png)
Reference table of options for areas of activity of employers.

5. EMPLOYERS_INDUSTRIES [Here](https://github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/Tables/Employers_industries.png)
An additional table that exists to organize the connection between employers and their areas of activity.

The data used for the analysis contains information from 49190 vacancies, 23501 employers and 1362 regions.

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)

### Stages of work on the project

The project was carried out in several stages:

* Stage 1. Selecting the required libraries

  - Libraries for working with SQL queries: pandas, sqlalchemy, psycopg2
  - Visualization libraries: seaborn, plotly.express, plotly.graph_objects
  - Libraries for displaying plotly plots via nbviewer.org: plotly.offline, plotly.io as pio

* Stage 2. Forming a database connection
 
  To connect to the data bose, the **query_func** function was created, which ensured that a query was sent using sqlalchemy and the result returned as a DateFrame.

* Stage 3. Preliminary data analysis and familiarization

  It included an acquaintance with datasets, its features, and the sizes of the main datasets (vacancies, employers, areas, industries) were determined.

* Stage 4. Detailed analysis of vacancies

  The presence of vacancies by region, the presence of indications of the level of salary and its average and median values, options for combining the type of work schedule and type of employment, and work experience requirements were determined. Some of the results for improved perception are visualized in graphs.

* Stage 5. Employer Analysis

  The number of vacancies for each of the employers, including the regions, the presence of the indicated field of activity was determined, the employers involved in software development were separately determined, and the availability of vacancies for the most top employer - Yandex in million-plus cities, data on which were obtained using html -request.

* Stage 6. Subject analysis (vacancies for DataScience);

Determined the total number of vacancies for data scientists, how many of these vacancies are suitable for junior DS specialists, how often knowledge of SQL, Poostgres and Python is required for DS specialists, how many key skills are required on average and what is the level of the proposed salary fees for data scientists depending on experience.

* Stage 7. Drawing conclusions and uploading to GitHub.

Conclusions are presented in each block, at stage 7 conclusions are made about what questions arose during the analysis and what further vectors of data study were identified. As a demonstration, a data study was conducted to answer some of the questions that arose (assessment of the impact on the expected salary of the level of experience and type of work schedule; assessment of the dependence of the result of the analysis of the sign of wages, the level of required experience on the field of activity, using the example of Yandex for vacancies in the field of DS) .

Interactive plots are presented 
[Link to NBViewer includes plots](https://nbviewer.org/github.com/EkaterinaArsa/DS_projects/blob/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)/HHru%20analysis(sql%2Bpython%2Bvisualization).ipynb)


:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)

### Results and preliminary conclusions
**Conclusions on preliminary data analysis:**
  - In the schema (public) presented to us in the database (project_sql) there are 5 tables: vacancies, employers, areas, industries and employers_industries. They provide data on 49197 vacancies (according to the vacancies table), 23501 employers (according to the employers table), 1362 regions (cities) (according to the areas table) and 294 fields of activity (according to the industries table). The employers_industries table is auxiliary and shows the relationship between employers and their fields of activity.

**Conclusions on the detailed analysis of vacancies:**
  - The largest number of vacancies falls on large cities. IN . TOP-5 included: in Russia: Moscow - 5333 vacancies, St. Petersburg - 2851 vacancies, Novosibirsk - 2006 vacancies; in the CIS Minsk - 2112 vacancies, Alma-Ata - 1892 vacancies.

  - In more than half of the cases (24,073 out of 49,197), the vacancies contain a minimum and/or maximum level of expected wages.

  - The average values of the "salary fork" are in the range from 71065 to 110537. But given the large number of vacancies with unspecified salary levels, these figures need further adjustment and study. In addition, there are likely to be multiple outliers for this trait.

  - Most of the vacancies are full-time and full-time (35,367 vacancies), fewer offer full-time remote work (7,802 vacancies). The shift type of work schedule is not offered for internships and part-time employment. !It is interesting to see how the type of work schedule and employment is related to the required experience and affects the salary!.

  - Required work experience mainly in the range of 1-3 years (53.2%, 26152 vacancies), less often - 3-6 years (29.5%, 14511 vacancies). Applicants without work experience are ready to accept in 7197 cases (14.6%), in 1337 vacancies more than 6 years of work experience is required (2.72%).

**Conclusions based on the results of the analysis of employers:**

  - Analysis of data on employers showed that in terms of the number of vacancies, the TOP-5 includes such "giants" as Yandex (1933 vacancies), Rostelecom (491 vacancies), Tinkoff (444 vacancies), Sberbank (428 vacancies) and Gazpromneft (331 vacancies) ). This can demonstrate both the active growth of these companies and the high "turnover" of personnel in them. So the Yandex company has vacancies in 16 million-plus cities: Moscow, St. Petersburg, Yekaterinburg, Nizhny Novgorod, Novosibirsk, Voronezh, Krasnodar, Samara, Ufa, Kazan, Perm, Rostov-on-Don, Volgograd, Krasnoyarsk, Chelyabinsk, Omsk (in descending order of the number of vacancies);

  - Analysis of data on employers showed that in terms of the number of vacancies, the TOP-5 includes such "giants" as Yandex (1933 vacancies), Rostelecom (491 vacancies), Tinkoff (444 vacancies), Sberbank (428 vacancies) and Gazpromneft (331 vacancies) ). This can demonstrate both the active growth of these companies and the high "turnover" of personnel in them. Thus, Yandex has vacancies in 16 million-plus cities, the employment market in which is usually quite saturated;

  - Across Russia, most employers with no vacancies are concentrated in the Moscow Region (75 companies), Krasnodar Territory (19 companies) and, unexpectedly, in the Rostov Region (18 companies). Which shows a high degree of saturation of jobs with personnel in these regions;

  - Among the companies with vacancies in various regions, Yandex (vacancies in 181 regions) and Rostelecom (vacancies in 153 regions) stand out significantly, which is probably due to the active growth of these giant companies and constant staff turnover, as well as (! NEED TO SPECIFY!) the possibility of remote work. Unexpectedly, the top five included: such a company as Spetsremont, due to its vastness (116 regions with vacancies), as well as little-known IP "Polyakov Denis Ivanovich" (due to the remote form of work on processing telephone numbers and massive dissatisfaction of employees with the level of wages) ( vacancies in 88 regions) and OOO EFIN (due to an extensive network of branches in more than 500 cities and mass dissatisfaction of employees with the organization of the labor process and wages) (vacancies in 71 regions);

  - In the data presented, 8419 employers (35.8%) do not have information about the field of activity, which may make it difficult for applicants to decide on a response to a vacancy. At the same time, many companies provide information on several areas of activity;

  - Software development is carried out by 3553 companies (15.1%) from the list of employers (!it would be interesting to assess which areas of activity are most represented among employers!), the employment market in which is usually quite saturated;

  - Across Russia, most employers with no vacancies are concentrated in the Moscow Region (75 companies), Krasnodar Territory (19 companies) and, unexpectedly, in the Rostov Region (18 companies). Which probably shows a high degree of job saturation in these regions. !It would be interesting to look at the ratio of the number of vacancies, employers in these regions!;

  - Among the companies with vacancies in various regions, Yandex (vacancies in 181 regions) and Rostelecom (vacancies in 153 regions) stand out significantly, which is probably due to the active growth of these giant companies and constant staff turnover. Unexpectedly, the top five included: such a large company as Spetsremont (116 regions with vacancies), as well as little-known IP "Polyakov Denis Ivanovich" (due to the remote form of work on processing telephone numbers and massive dissatisfaction of employees with the level of wages) (vacancies in 88 regions ) and OOO EFIN (due to an extensive network of branches in more than 500 cities and massive dissatisfaction of employees with the organization of the labor process and wages) (vacancies in 71 regions).  
**Conclusions on subject analysis (vacancies for DataScience):**

  - 1771 vacancies (36% of the total number of vacancies) are related to working with data;

  - Among the vacancies for data scientists, 51 (2.9%) are suitable for Junior level applicants;

  - On average, 6-7 skills are required for data scientists, while 201 (11.3%) contain requirements for key skills in using SQL and Postres, and 351 (19.8%) require knowledge of Python;

  - At the same time, the average level of the proposed salary for such specialists (DS) depends on experience: for applicants without experience, it is at the level of 74643 rubles, with experience from 1 to 3 years - 139675 rubles, with experience of 3-6 years, the average estimated salary is 243115 rubles. In the proposed data, there are no vacancies with requirements for the duration of experience of more than 6 years.

**Conclusions based on the result of additional research:**

  - the highest level of wages are employees with more than 6 years of experience and working on a rotational basis. Surprisingly, for employees with more than 6 years of experience and on a rotational basis, the salary level is significantly lower than for those with less than 6 years of experience. Probably, there is a presence of "heterogeneous" vacancies. It is necessary to clearly divide vacancies by areas of activity and then conduct a comparative analysis separately for each area.

  - In the vacancies from Yandx in 1475, no experience is required, 380 vacancies for specialists with 1-3 years of experience, 72 vacancies for applicants with 3-6 years of experience, 6 vacancies for specialists with more than 6 years of experience.

  - The median estimated salary at Yandex depends on the region. The maximum is in Moscow (51,000 rubles), the minimum is up to 15,000 in many regions (Kurgan, Krasnodar, Kostroma, etc.).

  - There is no direct dependence of the level of wages on work experience.
   
    - Yandex requires specialists in DS who have experience from 1 to 3 years (3 vacancies) and more than 3-6 years (6 vacancies). There are no vacancies for Junior and professionals with more than 6 years of experience. Thus, Yandex has rather high requirements for the level of experience for candidates in this specialty. DS specialists with experience over 6 years are not available at all in vacancies (as we noted above), this is due to the fact that there are only a few of them, they are known in this field and they are invited to the position directly.

    - The salary for DS specialists at Yandex is not indicated, which indicates its dependence on the results of the interview and that candidates are attracted by the image of the company, and not the established salary level&

    **The results shown indicate significant differences for each occupational area and should not be based on generalized data.**

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)

## Used libraries
* Python (3.9):
    * [numpy (1.23.4)](https://numpy.org)
    * [pandas (1.5.2)](https://pandas.pydata.org)
    * [SQLAlchemy (2.0.3)](https://www.sqlalchemy.org/)
    * [psycopg2 (2.9.5)](https://www.psycopg.org/)
    * [plotly(5.11.0) модули  plotly.express и plotly.offline](https://plotly.com/)
    * [seaborn(0.12.1)](https://seaborn.pydata.org/)

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)

## Project uploading

```
git clone https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)
```

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)

## Application of project
Total information (code) about the work is presented in the jupyter notebook HHru_analysis(sql+python+visualization).ipynb.

## Autors

* Arsenteva Ekaterina

[Instagramm](https://www.instagram.com/takayakasya?utm_source=qr) 

[VK](https://vk.com/id8747545 )

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)

## Conclusions

This project has identified a number of features that need pre-treatment:

  - First of all, salary attributes (salary_from, salary_to) of the vacancies table. There are multiple gaps in this feature, and clear outliers;

  - In the names of the regions (name) of the areas table, there are records that do not give accurate information (for example, "Russia" is indicated as the region), which can distort statistics by regions;

  - Many employers (industries table) do not have fields of activity (name).

  Also, during the study, a number of questions arose that need further study.

:arrow_up:[To table of contents](https://github.com/EkaterinaArsa/DS_projects/tree/master/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B0%D0%BA%D0%B0%D0%BD%D1%81%D0%B8%D0%B9%20%D0%BD%D0%B0%20HeadHunter2%20(sql%2Bpython%2Bvisualization)#table-of-contents)