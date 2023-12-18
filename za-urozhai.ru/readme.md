## Название сайта: za-urozhai.ru

### 1. О чём сайт

"За урожай" - муниципальная газета; выпускается в Шумячском районе Смоленской области.

### 2. Характеристики по данным *ArchiveReady*
![ArchiveReady_Za_Urozhai](https://github.com/DukeNukem4ever/DemoGit/assets/31654733/fa92fd90-25d6-47ed-967e-25c4376404c5)

### 3. Характеристики по *metawarc*

#### 3.1. Код, который был нужен для реализации функций по *metawarc*

`metawarc metadata za-urozhai.ru.warc` - извлекает метаданные из ".warc"-файла; возвращает json-строки по каждому найденному файлу.

`metawarc analyze za-urozhai.ru.warc` - анализ на обнаружение типов данных, соответствующих стандарту MIME.

`metawarc index za-urozhai.ru.warc` - генерация базы данных с метаданными в формате ".db"

`metawarc export -t content -o content.jsonl za-urozhai.ru.warc` - экспорт HTML-содержания веб-сайта в формате jsonl.

`metawarc stats -m mimes` - получение информации о частоте типов данных, соответствующих стандарту MIME.

`metawarc stats -m exts` - получение информации о частоте типов расширений данных.

#### 3.2. Сравнительная таблица

##### 3.2.1 Информация по расширениям файлов

| extension | size      | count |
|-----------|-----------|-------|
|           | 275004503 | 14487 |
| bmp       | 7155258   |     2 |
| css       | 240797    |     4 |
| eot       | 332130    |     2 |
| html      | 34273     |     1 |
| html\%22  | 2571      |     3 |
| jpeg      | 35038287  |   585 |
| jpeg\%22  | 19711     |    23 |
| jpg       | 902172178 |  6885 |
| jpg\%22   | 246816    |   288 |
| js        | 207224    |    14 |
| php       | 1878904   |    15 |
| png       | 37909358  |   134 |
| png\%22   | 5999      |     7 |
| svg       | 444686    |     1 |
| ttf       | 165864    |     1 |
| txt       | 731       |     2 |
| woff      | 98340     |     1 |
| woff2     | 77414     |     1 |
| xml       | 155004    |     9 |


##### 3.2.2 Информация по MIME-типам данных

| mime                               | size      | count |
|------------------------------------|-----------|-------|
| None                               | 77414     |     1 |
| application/json; charset=UTF-8    | 28881069  |  5230 |
| application/rss+xml; charset=UTF-8 | 16844339  |  2029 |
| application/vnd.ms-fontobject      | 332130    |     2 |
| application/x-font-ttf             | 165864    |     1 |
| application/x-font-woff            | 98340     |     1 |
| application/x-javascript           | 207224    |    14 |
| application/xml                    | 1350      |     1 |
| application/xml; charset=UTF-8     | 153366    |     7 |
| image/jpeg                         | 936692870 |  6905 |
| image/png                          | 37872500  |   130 |
| image/svg+xml                      | 444686    |     1 |
| image/x-ms-bmp                     | 7155258   |     2 |
| text/css                           | 240797    |     4 |
| text/html                          | 1873368   |     6 |
| text/html; charset=UTF-8           | 225561536 |  6994 |
| text/plain; charset=utf-8          | 435       |     1 |
| text/plain;charset=UTF-8           | 240       |     1 |
| text/xml; charset=UTF-8            | 4587262   |  1135 |

### 4. Анализ через *wpull*

`wpull http://za-urozhai.ru/ --strip-session-id --no-check-certificate --no-robots --span-hosts --page-requisites --sitemaps --inet4-only --timeout 20 --tries 3 --waitretry 5 --recursive --level inf --retry-connrefused --retry-dns-error --delete-after --warc-append --warc-cdx -U "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:101.0) Gecko/20100101 Firefox/101.0" -d -a za-urozhai.ru/za-urozhai.ru.log --database za-urozhai.ru/sitearchive-za-urozhai.ru.db --warc-file "za-urozhai.ru/za-urozhai.ru" --warc-header "operator: No Name" --warc-header "downloaded-by: Student"  --domains za-urozhai.ru --concurrent 4`

### 5. Выводы и интерпретации

Как показывают сравнительные таблицы, в структуре сайта содержится очень много файлов формата jpg и jpeg. Также присутствует файл с аномальным расширением, где на конце стоят символы "\%22". Это может указывать на недостаточную целость некоторых файлов. Либо они не до конца прогрузились, либо в них присутствует какая-то другая ошибка. 

Самый распространённый тип MIME - формат "text/html"; на втором месте после него стоит тип изобраений формата "jpeg".

По результатам обработки через ArchiveReady общий коэффициент качества архивации данного сайта составляет 79% благодаря очень высоким параметрам согласованности (Cohesion) и соответствия стандартам (Standards Compliance).

Параметр доступности (Accesibility) держится на приемлемом уровне в 60% - следовательно, не все данные были в достаточной степени обработаны. Количество выкачанных ссылок и медиафайлов довольно низкое, что вполне может говорить о проблематичности извлечения файлов определённого типа.

Полностью выкачать все метаданные не получилось, однако того, что было получено, вполне хватает для наличия общего представления о данном веб-сайте.
