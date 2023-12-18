## Название сайта: gagarin-gazeta.ru

### 1. О чём сайт

"ГЖАТСКИЙ ВЕСТНИК" - общественно-политическая газета, выпускаемая в г. Гагарин с 27 февраля 1918 года. Выходит один раз в неделю по пятницам. Основные темы — новости политической и социально-экономической жизни Гагарина, образования, культуры, медицины, спорта. Кроме этого, на страницах газеты печатаются все официальные документы администраций и совета депутатов района, города и сельских поселений.

### 2. Характеристики по данным *ArchiveReady*
![image](https://github.com/DukeNukem4ever/DemoGit/assets/31654733/6981c6d0-c91b-4b66-8ebd-3007bb7f0aee)

### 3. Список файлов в папке:

* *gagarin-gazeta_analyze.txt* (файл, полученный в результате команды `metawarc analyze gagarin-gazeta.ru.warc`)

* *gagarin-gazeta_json.rar* (архив с json-файлов, полученный в ходе экспорта содержания страниц через `metawarc export -t content -o gagarin-gazeta.jsonl gagarin-gazeta.ru.warc`)

* *gagarin-gazeta_metadata.jsonl* (json-файл, полученный через команду `metawarc metadata --output gagarin-gazeta_metadata.jsonl gagarin-gazeta.ru.warc`)

* *gagarin-gazeta_stats_ext.txt* (текстовая таблица с частотой расширений, извлечённая из файла *metawarc.db* через код `metawarc stats -m exts`)

* *gagarin-gazeta_stats_mimes.txt* (текстовая таблица с частотой MIME-типов данных, извлечённая из файла *metawarc.db* с помощью кода `metawarc stats -m mimes`)

* *metawarc.db* (база данных SQL с метаданными, полученная методом `metawarc index gagarin-gazeta.ru.warc`)

### 4. Характеристики по *metawarc*

#### 4.1. Код, который был нужен для реализации функций по *metawarc*

`metawarc metadata gagarin-gazeta.ru.warc` - извлекает метаданные из ".warc"-файла; возвращает json-строки по каждому найденному файлу.

`metawarc analyze gagarin-gazeta.ru.warc` - анализ на обнаружение типов данных, соответствующих стандарту MIME.

`metawarc index gagarin-gazeta.ru.warc` - генерация базы данных с метаданными в формате ".db"

`metawarc export -t content -o content.jsonl gagarin-gazeta.ru.warc` - экспорт HTML-содержания веб-сайта в формате jsonl.

`metawarc stats -m mimes` - получение информации о частоте типов данных, соответствующих стандарту MIME.

`metawarc stats -m exts` - получение информации о частоте типов расширений данных.

#### 4.2. Сравнительная таблица

##### 4.2.1 Информация по расширениям файлов

| extension         | size      | count |
|-------------------|-----------|-------|
|                   | 855280087 | 21950 |
| css               | 152930    |     7 |
| doc               | 79096     |     1 |
| eot               | 76936     |     2 |
| gif               | 88203     |     8 |
| href+             | 42813     |     1 |
| href+'            | 411       |     1 |
| iterator          | 85627     |     2 |
| jpeg              | 67783159  |   456 |
| jpg               | 757438762 |  3634 |
| jpg\%22           | 32487     |    39 |
| js                | 412250    |    18 |
| mp3               | 42814     |     1 |
| pdf               | 627696    |     2 |
| pdf\%22           | 833       |     1 |
| php               | 1102979   |    11 |
| png               | 91256839  |   234 |
| png\%22           | 8330      |    10 |
| ru                | 42931     |     1 |
| ru\%22            | 1666      |     2 |
| svg               | 202392    |     1 |
| to-json           | 42814     |     1 |
| ttf               | 80895     |     1 |
| txt               | 409       |     1 |
| url               | 42814     |     1 |
| url-search-params | 42813     |     1 |
| webgl             | 42813     |     1 |
| woff              | 44670     |     1 |
| worker            | 42814     |     1 |
| xml               | 3960848   |  1320 |
| zip               | 42814     |     1 |

##### 4.2.2 Информация по MIME-типам данных

| mime                               | size      | count |
|------------------------------------|-----------|-------|
| application/javascript             | 412250    |    18 |
| application/json; charset=UTF-8    | 27524738  |  2600 |
| application/msword                 | 79096     |     1 |
| application/pdf                    | 584882    |     1 |
| application/rss+xml; charset=UTF-8 | 5557314   |  1352 |
| application/vnd.ms-fontobject      | 76936     |     2 |
| font/ttf                           | 80895     |     1 |
| font/woff                          | 44670     |     1 |
| image/gif                          | 2577      |     6 |
| image/jpeg                         | 824761189 |  4042 |
| image/png                          | 92182699  |   229 |
| image/svg+xml                      | 202392    |     1 |
| text/css                           | 110117    |     6 |
| text/html                          | 604       |     2 |
| text/html; charset=UTF-8           | 818911485 | 17026 |
| text/html; charset=utf-8           | 48964     |     1 |
| text/html; charset=windows-1251    | 876       |     4 |
| text/plain; charset=utf-8          | 409       |     1 |
| text/plain;charset=windows-1251    | 220       |     1 |
| text/xml                           | 1285      |     1 |
| text/xml; charset=UTF-8            | 4559784   |  1096 |
| text/xml; charset=utf-8            | 3959563   |  1319 |

### 5. Анализ через *wpull*

`wpull http://gagarin-gazeta.ru/ --strip-session-id --no-check-certificate --no-robots --span-hosts --page-requisites --sitemaps --inet4-only --timeout 20 --tries 3 --waitretry 5 --recursive --level inf --retry-connrefused --retry-dns-error --delete-after --warc-append --warc-cdx -U "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:101.0) Gecko/20100101 Firefox/101.0" -d -a gagarin-gazeta.ru/gagarin-gazeta.ru.log --database gagarin-gazeta.ru/sitearchive-gagarin-gazeta.ru.db --warc-file "gagarin-gazeta.ru/gagarin-gazeta.ru" --warc-header "operator: No Name" --warc-header "downloaded-by: Student"  --domains gagarin-gazeta.ru --concurrent 4`

### 6. Выводы и интерпретации

Как показывают сравнительные таблицы, в структуре сайта содержится очень много файлов формата jpg и xml. 

Самый распространённый тип MIME - формат "text/html".

По результатам обработки через ArchiveReady общий коэффициент качества архивации данного сайта составляет 82% ввиду высоких параметров согласованности (Cohesion) и соответствия Standards Compliance.

Параметр Accesibility держится на приемлемом уровне - это говорит о том, что не все метаданные были корректно распознаны. Количество выкачанных ссылок и медиафайлов довольно низкое, что вполне может говорить о проблематичности извлечения файлов определённого типа.

Полностью выкачать все метаданные не получилось, поэтому взаимодействие сервиса с контентом имеет весьма ограниченный характер.
