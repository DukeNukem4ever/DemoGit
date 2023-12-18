## Название сайта: desna67.ru

### 1. О чём сайт

«ДЕСНА» - газета муниципального образования, которая выпускается в гор. округе Десногорск Смоленской области.

### 2. Характеристики по данным ArchiveReady

![ArchiveReady_Desna_67](https://github.com/DukeNukem4ever/DemoGit/assets/31654733/d720e486-5ccb-493b-a5b5-ce604530d3cf)

### 3. Характеристики по данным *metawarc*

#### 3.1. Код, который был нужен для реализации функций по metawarc

`metawarc metadata desna67.ru.warc` - извлекает метаданные из ".warc"-файла; возвращает json-строки по каждому найденному файлу.

`metawarc analyze desna67.ru.warc` - анализ на обнаружение типов данных, соответствующих стандарту MIME.

`metawarc index desna67.ru.warc` - генерация базы данных с метаданными в формате ".db"

`metawarc export -t content -o content.jsonl desna67.ru.warc` - экспорт HTML-содержания веб-сайта в формате jsonl.

`metawarc stats -m mimes` - получение информации о частоте типов данных, соответствующих стандарту MIME.

`metawarc stats -m exts` - получение информации о частоте типов расширений данных.

#### 3.2. Сравнительная таблица

##### 3.2.1 Информация по расширениям файлов

| extension | size       | count |
|-----------|------------|-------|
|           | 668053977  | 23724 |
| css       | 1089608    |    30 |
| eot       | 759623     |     7 |
| gif       | 87932      |     3 |
| jpeg      | 28031014   |   303 |
| jpg       | 2269686410 | 11552 |
| js        | 2491164    |    40 |
| mp4       | 152004820  |     4 |
| php       | 1292072    |    14 |
| png       | 205717427  |   564 |
| svg       | 3354928    |     7 |
| tif       | 10900339   |    21 |
| ttf       | 757622     |     7 |
| txt       | 1362       |     4 |
| woff      | 406830     |     6 |
| woff2     | 328994     |     6 |
| xml       | 61328      |     6 |

##### 3.2.2 Информация по MIME-типам данных

| mime                               | size       | count |
|------------------------------------|------------|-------|
| None                               | 328994     |     6 |
| application/json; charset=UTF-8    | 7866116    |  2213 |
| application/rss+xml; charset=UTF-8 | 10551883   |  1780 |
| application/vnd.ms-fontobject      | 759623     |     7 |
| application/x-font-ttf             | 757622     |     7 |
| application/x-font-woff            | 406830     |     6 |
| application/x-javascript           | 2433258    |    38 |
| application/xml                    | 2700       |     2 |
| image/gif                          | 87932      |     3 |
| image/jpeg                         | 2297542754 | 11847 |
| image/png                          | 205717427  |   564 |
| image/svg+xml                      | 3354928    |     7 |
| image/tiff                         | 10550377   |     3 |
| text/css                           | 1089608    |    30 |
| text/html                          | 1248912    |     4 |
| text/html; charset=UTF-8           | 642714280  | 18033 |
| text/plain; charset=utf-8          | 776        |     2 |
| text/plain;charset=UTF-8           | 480        |     2 |
| text/xml; charset=UTF-8            | 7606130    |  1740 |
| video/mp4                          | 152004820  |     4


### 4. Анализ через *wpull*

`wpull http://desna67.ru/ --strip-session-id --no-check-certificate --no-robots --span-hosts --page-requisites --sitemaps --inet4-only --timeout 20 --tries 3 --waitretry 5 --recursive --level inf --retry-connrefused --retry-dns-error --delete-after --warc-append --warc-cdx -U "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:101.0) Gecko/20100101 Firefox/101.0" -d -a desna67.ru/desna67.ru.log --database desna67.ru/sitearchive-desna67.ru.db --warc-file "desna67.ru/desna67.ru" --warc-header "operator: No Name" --warc-header "downloaded-by: Student"  --domains desna67.ru --concurrent 4`

### 5. Выводы и интерпретации

Как показывают сравнительные таблицы, в структуре сайта содержится больше всего изображений в форматах jpg и png, если не включать файлы с пустым расширением.

Самый распространённый тип MIME - формат "text/html" в формате utf-8; на втором месте идут изображения в формате jpeg, которые весят больше всех остальных типов файлов вместе взятых.

По результатам обработки через ArchiveReady общий коэффициент качества архивации данного сайта составляет 71%; это было обеспечено очень высоким параметром согласованности (Cohesion), но при этом значение по соответствию стандартам (Standards Compliance) оказалось лишь немного выше среднего, что негативно повлияло на итоговую оценку.

Параметр Accesibility имеет весьма низкое значение - это говорит о том, что лишь часть метаданных была корректно распознана. Количество выкачанных ссылок и медиафайлов довольно низкое, что вполне может говорить о проблематичности извлечения файлов определённого типа.

Полностью выкачать все метаданные не получилось, поэтому взаимодействие сервиса с контентом не является идеальным.
