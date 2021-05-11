# Netflix

## 1. Выбор темы и целевой аудитории
#### Тема - Netflix для российской аудитории. 
Назначение сервиса - предоставить пользователю стандартные возможности стримингового видеосервиса: просмотр кино, сериалов и краткой информации о контенте, наличие подборок, а конкретно реализованы такие разделы как ‘сериалы’, ‘фильмы’, ‘последнее’, ‘бесплатное’, удобная навигация по контенту с фильтрами, возможность осуществлять поиск, оформление подписки, настройка личного кабинета.

#### Целевая аудитория - 3 млн. человек
Исходя из [данных](https://vc.ru/media/205039-kinopoisk-hd-rasskazal-o-rekordnyh-3-mln-smotryashchih-podpischikov-v-yanvare) о главных конкуретнах онлайн-кинотеатров на рынке России аудитория пользователей Netflix составит 3 млн. человек.

  [Анализ показателей Netflix в России](https://pro.similarweb.com/#/companyresearch/websiteanalysis/overview/website-performance/netflix.com/*/643/2020.01-2020.03?webSource=Total)

## 2. Расчет нагрузки

### Сетевой трафик на загрузку видео

|Параметр|Значение|Ссылка на источник|
| - | - | - |
|Аудитория|3 146 000|[pro.similarweb.com](https://pro.similarweb.com/#/companyresearch/websiteanalysis/overview/website-performance/netflix.com/*/643/2020.01-2020.03?webSource=Total)[vc.ru](https://vc.ru/media/205039-kinopoisk-hd-rasskazal-o-rekordnyh-3-mln-smotryashchih-podpischikov-v-yanvare)|
|Количество посетителей в сутки|1 000 000|[forbes.ru](https://www.forbes.ru/tehnologii/419761-my-otstaem-ot-netflix-na-gody-onlayn-kinoteatry-pozhalovalis-na-zaregulirovannost)|
|Время просмотра контента в сутки (в среднем)|3,2 часа|[pcmag.com](https://www.pcmag.com/news/us-netflix-subscribers-watch-32-hours-and-use-96-gb-of-data-per-day)|
|Используемые данные подписчиком в сутки (в среднем)|9,6 Гб||
|Диапазон битрейта видео|1750 кбит/сек - 16000 кбит/сек|[howtogeek.com](https://www.howtogeek.com/338983/how-much-data-does-netflix-use/#:~:text=Most%20videos%20you%20play%20on,or%2059.940%20frames%20per%20second)|
|Примерное пиковое время и количество пользователей |9 вечера - 50% аудитории за день|[qz.com](https://qz.com/india/989659/netflix-nflx-peak-viewing-hours-are-very-different-in-india-and-argentina-compared-to-the-us-and-europe/#:~:text=Netflix's%20subscribers%20are%20setting%20their,by%20Netflix%E2%80%94the%20US%20included.)|
|Количество просматриваемых страниц в среднем|3,8|[pro.similarweb.com](https://pro.similarweb.com/#/companyresearch/websiteanalysis/overview/website-performance/netflix.com/*/643/2020.01-2020.03?webSource=Total)|
|Просмотр с ноутбука|85,58%||
|Просмотр с мобильного приложения|14,42%||

#### Соотношение использования памяти и качества контента (десктоп)
| Качество | Трафик |
| - | - |
|Low|0,3 Гб/час - 0.083 Мб/сек|
|Medium|0,7 Гб/час - 0.194 Мб/сек|
|Hight|3 Гб/час -  0.833 Мб/сек|
|HD quality|4.2 Гб/час - 1.167 Мб/сек|
|Ultra HD quality|7 Гб/час - 1.944 Мб/сек|

Источник: [help.netflix.com](https://help.netflix.com/en/node/87#:~:text=Watching%20TV%20shows%20or%20movies,each%20stream%20of%20HD%20video.)


#### Рекомендации по скорости
| Качество | Трафик |
| - | - |
|Low|0.5 Мбит/сек|
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
|Москва (40%) - 400 000 -> 1 280 000 часов/сутки|Ultra HD - 20% HD - 30% Hight - 20% Medium - 20 % Low - 10%|HD - 20% Hight - 30% Medium - 30 % Low - 20%|
|Регионы (60%) - 600 000 -> 1 920 000 часа/сутки|Ultra HD - 10% HD - 30% Hight - 30% Medium - 20 % Low - 10%|Hight - 30% Medium - 40 % Low - 30%|

Тогда расчетная нагрузка:
||Десктоп|Мобильный|
| :- | - | - |
|Москва|1 280 000 \* 0.8558 \* (0.2 \* 7 + 0.3 \*4.2 + 0.2 \* 3 + 0.2 \* 0,7 + 0.1 \* 0.3) = 3 757 304, 32 Гб|1 280 000 \* 0.1442 \* (0.2 \* 4.2 + 0.3 \* 3+ 0.3 \* 0,7 + 0.2 \* 0.3) = 370 997, 76 Гб|
|Регионы|1 920 000 \* 0.8558 \* (0.1 \* 7 + 0.3 \*4.2 + 0.3 \* 3 + 0.2 \* 0,7 + 0.1 \* 0.3) = 4 978 702, 08 Гб|1 920 000 \* 0.1442 \* (0.3 \* 3 + 0.4 \* 0,7 +0.3 \* 0.3) = 351 617, 28 Гб|

#### Итог: примерно 9 458 621, 44 Гб в день или 9 458, 62 Тб

### Загрузка приложения
Исходя из [анализа загрузки страницы Netflix](https://gtmetrix.com/reports/www.netflix.com/sRz0KiJW/):
3,1 МБ * 1 000 000 = 3 100 000 Гб в день

### Сетевой трафик
При использовании сервиса 1,5 минуты (только бизнес логика, без просмотра видео):
Статика - 6,5 МБ (22); Динамика - 190 МБ (642); Изображения - 24.3 МБ (906 запросов)

Пусть один пользователь тратит только на посещение страниц сервиса 30 минут в среднем в день, тогда трафик:

```
Трафик в день:
Статика: (6,5 / 1,5) * 30 * 1 000 000 = 130 000 Гб/сутки
Динамика: (190 / 1,5) * 30 * 1 000 000 = 3 800 000 Гб/сутки
Изображения: (24.3 / 1,5) * 30 * 1 000 000 = 486 000 Гб/сутки

Трафик во время пиковой нагрузки (в Гб/сек):
Статика: 6,5 / (1,5 * 60) * 500 000 = 324,9 Гб/сутки
Динамика: 190 / (1,5 * 60) * 500 000 = 9 500 Гб/сутки
Изображения: 24.3 / (1,5 * 60) * 500 000 = 1 215 Гб/сутки
```

### Запросы

Общее количество запросов в секунду (пусть одновременно находится 100 000 человек):
(22 + 642 + 906) / (1,5 * 60) * 100 000 = 1 744 444

Общее количество запросов в секунду в пиковое время(одновременно находится 500 000 человек):
(22 + 642 + 906) / (1,5 * 60) * 500 000 = 8 722 220

```
Запросы по типам:
Главная страница (пусть каждый пользователь в среднем заходит 3 раза на главную страницу):
(61 запрос / 6 секунд) * 1 000 000 * 3 / (24 * 60 * 60) = 353 rps
```

### Объем видео
На нетфликсе [содержится](https://www.whats-on-netflix.com/news/how-long-would-it-take-to-watch-all-of-netflix/) контента на 36 000 часов - 50 000 позиций (фильмов и сериалов). Сервис будет хранить исходники сериалов и фильмов. Пусть 40% контента занимают фильм, остальные 60% сериалы, которые весят гораздо больше, чем фильмы. Оригинальный контент, снятый на киностудии занимает очень большое место. Пусть фильм в среднем весит 3Тб, тогда сериал будет весить в среднем 50 Тб.

В итоге :
(0,4 \* 3 + 0,6 \* 50) \* 5817 = 181 590, 4 ТБ

Многовесовой оригинал фильма/серии не раздается пользователям, сначала он сжимается - например, форматом H.265 или HEVC - далее распределенно хранится по различным серверам, и только по запросу контент отдается по протоколам стриминга MPEG DASH или HLS.

Большинство контента на Нетфликсе [имеет framerate 24 кадра](https://www.howtogeek.com/338983/how-much-data-does-netflix-use/#:~:text=Most%20videos%20you%20play%20on,or%2059.940%20frames%20per%20second) в секунду, но также имеет место и framerate в 60 кадров в секунду.

Возьмем среднюю длительность контента - (фильмы 1,5 -2 часа и серии в сериалах 0,5 - 1час) - 1 час и рассчитаем для framerates и соответствующих quality (https://ru.tab-tv.com/?page\_id=161) видео их вес - (с помощью калькулятора [https://toolstud.io/video/filesize.php)](https://toolstud.io/video/filesize.php)

Качество **SD (480p)**

|Разрешение|Размер (частота кадров - 24)|Размер (частота кадров - 60)|
| - | - | - |
|720×480|583.19 МБ|1.46 ГБ|
|704×480|570.23 МБ|1.43 ГБ|
|352×480|285.12 МБ|712.79 МБ|
|720×576|699.83 МБ|1.75 ГБ|
|704×576|684.28 МБ|1.71 ГБ|
|352×576|342.14 МБ|855.35 МБ|
|640x480|518.39 МБ|1.3 ГБ|
|640x240|259.2 МБ|647.99 МБ|


Качество **HD**

|Разрешение|Размер (частота кадров - 24)|Размер (частота кадров - 60)|
| - | - | - |
|960×720|1.17 ГБ|2.92 ГБ|
|1440×720|1.75 ГБ|4.37 ГБ|
|2560x1440|2.71 ГБ|15.55 ГБ|


Качество **Full HD (1080p)**

|Разрешение|Размер (частота кадров - 24)|Размер (частота кадров - 60)|
| - | - | - |
|1920x1080|2.51 ГБ|6.26 ГБ|
|1440x1080|1.88 ГБ|4.7 ГБ|
|2160x1080|2.82 ГБ|7.05 ГБ|
|2560x1080|3.34 ГБ|8.35 ГБ|
|1728×1080|2.25 ГБ|5.64 ГБ|


Качество **Ultra HD**

|Разрешение|Размер (частота кадров - 24)|Размер (частота кадров - 60)|
| - | - | - |
|3840x2160|6.74 ГБ|16.85 ГБ|
|4096x2160|7.19 ГБ|17.97 ГБ|
|4096x1716|5.71 ГБ|14.28 ГБ|


Итого: Одно видео занимает ~155,81 Гб

36 000 часов \* 155,81 Гб = 5 609 160 Гб = 5 609,160 ТБ

Итого: 181 590, 4 + 5 609 = 187 199, 56 ТБ


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
(boolean)1 = 1935 б -> 50 000 * 1935 = 96 750 000 б

Movies:
(id) 4 + (video) 128 + (content_id) 4 = 136 б
-> 20 000 * 136 = 2 720 000 б
`
Tv_shows:
(id) 4 + (seasons) 4 + (content_id) 4 = 12 б
-> 30 000 * 12 = 360 000 б

Seasons:
(id) 4 + (number) 4 + (episodes) 4 +
(tv_show_id) 4 = 16 б -> 30 000 * 3 * 16 = 1 440 000 б

Episodes:
(id) 4 + (number) 4 + (name) 128 + (video)
128 + (description - avg) 256 + (poster)
128 + (season_id) 4 = 16 б -> 30 000 * 10 *
16 = 4 800 000 б

Content_genre:
(content_id) 4 + (genre_id) 4 = 8 б -> 30 000 * 2 * 8 = 480 000 б

Genres:
(id) 4 + (name) 64 = 68 б -> 40 * 68 = 2 720 б

Content_actor:
(content_id) 4 + (actor_id) 4= 8 б -> 30 000
* 15 * 8 = 3 600 000 б

Actors:
(id) 4 + (name) 64 = 68 б -> 300 000 * 68 = 20 400 000 б

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
328 б -> 3 146 000 * 328 = 1 031 888 000 б

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


На основе статистики о популярном контенте будут выделяться мелкие CDN, на
которых будут располагаться закэшированные наиболеепопулярные фильмы и
сериалы. Пусть данные о популярном контенте будутобновляться раз в сутки. Возможно
даже объединение мелких CDN в кластеры - тогда кэшированныйпопулярный контент
будет распределяться по кластеру. Также можно и объединятьв кластеры большие CDN
сервера - на них будет храниться весь видеоконтентсервиса. Кластеры CDN
располагаются у ISP (провайдеры интернета) или в IXP(точки обмена трафиком).

Для хранения аналитических данных будет использоваться ClickHouse.




