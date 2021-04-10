# Netflix

## 1. Выбор темы и целевой аудитории
#### Тема - Netflix для российской аудитории. 
Сервис предоставляет пользователю возможность оформить подписку и смотреть фильмы/сериалы/телешоу в высоком качестве, без рекламы. На начало 2021 года более [900](http://unogs.com/search/?start_year=1900&end_year=2021&start_rating=0&end_rating=10&audio=Russian&subtitle=&type=&genrelist=&countrylist=21,23,26,29,33,307,45,39,327,331,334,265,337,336,269,267,357,65,67,392,268,400,402,408,412,447,348,270,73,34,425,432,46,78&audiosubtitle_andor=and&orderby=Relevance) сериалов/фильмов/мультфильмов дублированы на русский язык. Еще порядка 40 мультфильмов не содержат диалогов вообще, то есть, будут понятны любому человеку, а также более 100 картин изначально сняты на русском. Навигация по сервису включает в себя главную подборку, раздел фильм, раздел сериалов, последнее и личный список избранного контента пользователя. Также есть возможность поиска контента по названию, жанрам и людям.

#### Целевая аудитория - 3 млн. человек
Исходя из [данных](https://vc.ru/media/205039-kinopoisk-hd-rasskazal-o-rekordnyh-3-mln-smotryashchih-podpischikov-v-yanvare) о главных конкуретнах онлайн-кинотеатров на рынке России аудитория пользователей Netflix составит 3 млн. человек.

  [Анализ показателей Netflix в России](https://pro.similarweb.com/#/companyresearch/websiteanalysis/overview/website-performance/netflix.com/*/643/2020.01-2020.03?webSource=Total)

## 2. Расчет нагрузки

### Загрузка видео

|Параметр|Значение|Ссылка на источник|
| - | - | - |
|Аудитория|3 146 000|[pro.similarweb.com](https://pro.similarweb.com/#/companyresearch/websiteanalysis/overview/website-performance/netflix.com/*/643/2020.01-2020.03?webSource=Total)[vc.ru](https://vc.ru/media/205039-kinopoisk-hd-rasskazal-o-rekordnyh-3-mln-smotryashchih-podpischikov-v-yanvare)|
|Количество посетителей в сутки|100 000|[forbes.ru](https://www.forbes.ru/tehnologii/419761-my-otstaem-ot-netflix-na-gody-onlayn-kinoteatry-pozhalovalis-na-zaregulirovannost)|
|Время просмотра контента в сутки (в среднем)|3,2 часа|[pcmag.com](https://www.pcmag.com/news/us-netflix-subscribers-watch-32-hours-and-use-96-gb-of-data-per-day)|
|Используемые данные подписчиком в сутки (в среднем)|9,6 Гб||
|Диапазон битрейта видео|1750 кбит/сек - 16000 кбит/сек|[howtogeek.com](https://www.howtogeek.com/338983/how-much-data-does-netflix-use/#:~:text=Most%20videos%20you%20play%20on,or%2059.940%20frames%20per%20second)|
|Примерное пиковое время и количество пользователей |9 вечера - 50% аудитории|[qz.com](https://qz.com/india/989659/netflix-nflx-peak-viewing-hours-are-very-different-in-india-and-argentina-compared-to-the-us-and-europe/#:~:text=Netflix's%20subscribers%20are%20setting%20their,by%20Netflix%E2%80%94the%20US%20included.)|
|Пиковая разовая нагрузка (с учетом среднего битрейта)|0,5 \* 100 000 чел \* 6350 кбит/сек = 317,5 Гб/сек||
|Количество просматриваемых страниц в среднем|3,8|[pro.similarweb.com](https://pro.similarweb.com/#/companyresearch/websiteanalysis/overview/website-performance/netflix.com/*/643/2020.01-2020.03?webSource=Total)|
|Просмотр с ноутбука|85,58%||
|Просмотр с мобильного приложения|14,42%||

#### Соотношение использования памяти и качества контента (десктоп)

|Low|0,3 Гб/час - 0.083 Мб/сек|
| - | - |
|Medium|0,7 Гб/час - 0.194 Мб/сек|
|Hight|3 Гб/час -  0.833 Мб/сек|
|HD quality|4.2 Гб/час - 1.167 Мб/сек|
|Ultra HD quality|7 Гб/час - 1.944 Мб/сек|

Источник: [help.netflix.com](https://help.netflix.com/en/node/87#:~:text=Watching%20TV%20shows%20or%20movies,each%20stream%20of%20HD%20video.)


#### Рекомендации по скорости
|Low|0.5 Мбит/сек|
| - | - |
|Medium|1.5 Мбит/сек|
|Hight|3.0 Мбит/сек|
|HD quality|5.0 Мбит/сек|
|Ultra HD quality|25 Мбит/сек|

Источник: [help.netflix.com](https://help.netflix.com/en/node/306)


#### Средняя скорость в России на 2021

||Десктоп|Мобильный|
| :- | - | - |
|Москва|81.94 Мбит/сек|23.64 Мбит/сек|
|Остальные региона (0.66(6) \* Москва)|54.63 Мбит/сек|15.76 Мбит/сек|

Источник: [speedtest.ne ](https://www.speedtest.net/global-index/russia)[m24.ru](https://www.m24.ru/news/tehnologii/28122020/147468)


Сделаем предположение о распределении аудитории по стране и использования качества контента:

||Десктоп (85.58%)|Мобильный (14.42%)|
| :- | - | - |
|Москва (40%) - 40 000 -> 128 000 часов/сутки|Ultra HD - 20% HD - 30% Hight - 20% Medium - 20 % Low - 10%|HD - 20% Hight - 30% Medium - 30 % Low - 20%|
|Регионы (60%) - 60 000 -> 192 000 часа/сутки|Ultra HD - 10% HD - 30% Hight - 30% Medium - 20 % Low - 10%|Hight - 30% Medium - 40 % Low - 30%|

Тогда расчетная нагрузка:
||Десктоп|Мобильный|
| :- | - | - |
|Москва|128 000 \* 0.8558 \* (0.2 \* 7 + 0.3 \*4.2 + 0.2 \* 3 + 0.2 \* 0,7 + 0.1 \* 0.3) = 375 730, 432 Гб|128 000 \* 0.1442 \* (0.2 \* 4.2 + 0.3 \* 3+ 0.3 \* 0,7 + 0.2 \* 0.3) = 37 099, 776 Гб|
|Регионы|192 000 \* 0.8558 \* (0.1 \* 7 + 0.3 \*4.2 + 0.3 \* 3 + 0.2 \* 0,7 + 0.1 \* 0.3) = 497 870, 208 Гб|192 000 \* 0.1442 \* (0.3 \* 3 + 0.4 \* 0,7 +0.3 \* 0.3) = 497 870, 208 Гб = 35 161,728 Гб|

#### Итог: примерно 945 862, 144 Гб в день или 945, 862 Тб

### Загрузка приложения
Исходя из [анализа загрузки страницы Netflix](https://gtmetrix.com/reports/www.netflix.com/sRz0KiJW/):
3,1 МБ * 100 000 = 310 000 Гб в день


### Объем видео
На нетфликсе [содержится](https://www.whats-on-netflix.com/news/how-long-would-it-take-to-watch-all-of-netflix/) контента на 36 000 часов - 50 000 позиций (фильмов и сериалов). Большинство контента на Нетфликсе [имеет framerate 24 кадра](https://www.howtogeek.com/338983/how-much-data-does-netflix-use/#:~:text=Most%20videos%20you%20play%20on,or%2059.940%20frames%20per%20second) в секунду, но также имеет место и framerate в 60 кадров в секунду.

Сервис будет хранить исходники сериалов и фильмов. Пусть 40% контента занимают фильм, остальные 60% сериалы, которые весят гораздо больше, чем фильмы. Оригинальный контент, снятый на киностудии занимает очень большре место. Пусть фильм в среднем весит 3Тб, тогда сериал будет весить в среднем 50 Тб.

В итоге :
(0,4 \* 3 + 0,6 \* 50) \* 5817 = 181 590, 4 Тб

Многовесовой оригинал фильма/серии не раздается пользователям, сначала он сжимается - например, форматом H.265 или HEVC - далее распределенно хранится по различным серверам, и только по запросу контент отдается по протоколам стриминга MPEG DASH или HLS. В процессе отдачи видео транскодируется, учитывая возможности устройства и скорость интернета пользователя. В итоге, пусть сжатие происходит с коэффициентом 1000:1[, тогда](https://en.wikipedia.org/wiki/High_Efficiency_Video_Coding) помимо оригинальных файлов будут также храниться + 181, 6 Тб.

Источники: [medium.com](https://medium.com/@narengowda/netflix-system-design-dbec30fede8d), [thecode.media](https://thecode.media/zapusk-kino/#tekst3),[habr.com](https://habr.com/ru/post/409583/), [thecode.media](https://thecode.media/zapusk-kino/#tekst3)

## 3. Логическая схема базы данных

![image](https://user-images.githubusercontent.com/60325113/113420396-ee46d700-93d1-11eb-88ca-727e0c0d63ff.png)

## 4. Физическая схема базы данных
Примерный расчет таблиц

```
Content: 
(id) 4 + (name) 128 + (original_name) 128
+ (description - avg) 1024 +
(short_description - avg) 512 + (rating) 4 +
(year)2 + (images)128 + (content_type)4 +
(boolean)1 = 1935 б -> 50 000 * 1935 = 96
750 000 б

Movies:
(id) 4 + (video) 128 + (content_id) 4 = 136 б
-> 20 000 * 136 =
2 720 000 б
`
Tv_shows:
(id) 4 + (seasons) 4 + (content_id) 4 = 12 б
-> 30 000 * 12 =
360 000 б

Seasons:
(id) 4 + (number) 4 + (episodes) 4 +
(tv_show_id) 4 = 16 б -> 30 000 * 3 * 16 = 1
440 000 б

Episodes:
(id) 4 + (number) 4 + (name) 128 + (video)
128 + (description - avg) 256 + (poster)
128 + (season_id) 4 = 16 б -> 30 000 * 10 *
16 = 4 800 000 б

Content_genre:
(content_id) 4 + (genre_id) 4 = 8 б -> 30
000 * 2 * 8 = 480 000 б

Genres:
(id) 4 + (name) 64 = 68 б -> 40 * 68 = 2
720 б

Content_actor:
(content_id) 4 + (actor_id) 4= 8 б -> 30 000
* 15 * 8 =
3 600 000 б

Actors:
(id) 4 + (name) 64 = 68 б -> 300 000 * 68 =
20 400 000 б

Content_country:
(content_id) 4 + (country_id) 4 = 8 б -> 30
000 * 2 * 8 = 480 000 б

Countries:
(id) 4 + (name) 64 = 68 б -> 120 * 68 = 8
160 б

Content_director: 
(content_id) 4 + (director_id) 4 = 8 б -> 30
000 * 1 * 8 = 240 000 б

Directors:
(id) 4 + (name) 64 = 68 б -> 3000 * 68 =
204 000 б

Users:
(id) 4 + (nickname) 64 + (email) 64 +
(password) 128 + (avatar) 64 + (role) 4 =
328 б -> 3 146 000 * 328 =
1 031 888 000 б

Rates:
(user_id) 4 + (content_id) 4 + (likes) 1 = 9 б
-> 10 000 000 * 9 = 90 000 000 б

Subscriptions:
(id) 4 + (owner) 4 + (expires) 8 + (is_paid) 1
+ (is_canceled) 1 = 18 б ->3 146 000 * 18 =
56 628 000 б

Sessions:
(id) 4 + (value) 64 + (expires) 8 + (user_id)
4 = 80 б ->3 146 000 * 80 = 251 680 000 б

Favourites:
 (user_id) 4 + (content_id) 4 + (created) 8 =
16 б -> 10 000 000 * 16 = 160 000 000 б

Итог: 1 721 680 000 б = 1,62493 Гб
```
Для хранения данных выберем базу PostgreSQL.
Контент будет храниться на CDN серверах. Расположитьих стоит преимущественно в
западной части страны - Москве, Питере, городах-миллионниках,а также на Дальнем
Востоке и т. д.


На основе статистики о популярном контенте будут выделятьсямелкие CDN, на
которых будут располагаться закэшированные наиболеепопулярные фильмы и
сериалы. Пусть данные о популярном контенте будутобновляться раз в сутки. Возможно
даже объединение мелких CDN в кластеры - тогда кэшированныйпопулярный контент
будет распределяться по кластеру. Также можно и объединятьв кластеры большие CDN
сервера - на них будет храниться весь видеоконтентсервиса. Кластеры CDN
располагаются у ISP (провайдеры интернета) или в IXP(точки обмена трафиком).

Для хранения аналитических данных будет использоватьсяClickHouse.


