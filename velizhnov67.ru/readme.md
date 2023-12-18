### Название сайта: "ВЕЛИЖСКАЯ НОВЬ"

### 1. О чём сайт

«Велижская новь» - газета муниципального образования Велижского района Смоленской области.

### 2. Характеристики по данным ArchiveReady

![ArchiveReady_Velizhnov_67](https://github.com/DukeNukem4ever/DemoGit/assets/31654733/d2eabc9b-dd6b-4d82-a415-9bc8e53b6109)

### 3. Характеристики по данным *metawarc*

#### 3.1. Код, который был нужен для реализации функций по metawarc

`metawarc metadata velizhnov67.ru.warc` - извлекает метаданные из ".warc"-файла; возвращает json-строки по каждому найденному файлу.

`metawarc analyze velizhnov67.ru.warc` - анализ на обнаружение типов данных, соответствующих стандарту MIME.

`metawarc index velizhnov67.ru.warc` - генерация базы данных с метаданными в формате ".db"

`metawarc export -t content -o content.jsonl velizhnov67.ru.warc` - экспорт HTML-содержания веб-сайта в формате jsonl.

`metawarc stats -m mimes` - получение информации о частоте типов данных, соответствующих стандарту MIME.

`metawarc stats -m exts` - получение информации о частоте типов расширений данных.

#### 3.2. Сравнительная таблица

##### 3.2.1 Информация по расширениям файлов

| extension        | size      | count |
|------------------|-----------|-------|
|                  | 181641438 |  7017 |
| \u0440\u0444\%22 | 891       |     1 |
| css              | 353863    |     5 |
| docx             | 16821     |     1 |
| eot              | 835665    |    11 |
| gisgkh\%22       | 891       |     1 |
| html\%22         | 891       |     1 |
| jpeg             | 22914043  |   541 |
| jpeg\%22         | 1782      |     2 |
| jpg              | 506607405 |  3564 |
| jpg\%22          | 19602     |    22 |
| js               | 320958    |     9 |
| mp4              | 16785642  |     1 |
| pdf              | 642141    |     4 |
| pdf\%22          | 7128      |     8 |
| php              | 3991      |     5 |
| png              | 53051761  |   201 |
| png\%22          | 8019      |     9 |
| ru\%22           | 7128      |     8 |
| smolensk\%22     | 891       |     1 |
| svg              | 1995056   |     8 |
| tif              | 706425    |     1 |
| ttf              | 586880    |     8 |
| txt              | 427       |     1 |
| webp             | 1189941   |    26 |
| woff             | 336070    |     8 |
| woff2            | 167377    |     3 |
| xml              | 107692    |     4 |

##### 3.2.2 Информация по MIME-типам данных

| mime                                                                    | size      | count |
|-------------------------------------------------------------------------|-----------|-------|
| application/json; charset=UTF-8                                         | 20242436  |  2831 |
| application/octet-stream                                                | 1090327   |    19 |
| application/pdf                                                         | 589102    |     3 |
| application/rss+xml; charset=UTF-8                                      | 4835864   |   745 |
| application/vnd.ms-fontobject                                           | 835665    |    11 |
| application/vnd.openxmlformats-officedocument.wordprocessingml.document | 16821     |     1 |
| application/x-javascript                                                | 320958    |     9 |
| image/jpeg                                                              | 529497391 |  4078 |
| image/png                                                               | 53049979  |   199 |
| image/svg+xml                                                           | 1995056   |     8 |
| image/tiff                                                              | 706425    |     1 |
| image/webp                                                              | 1189941   |    26 |
| text/css                                                                | 300824    |     4 |
| text/html; charset=UTF-8                                                | 153813158 |  2878 |
| text/plain                                                              | 280       |     1 |
| text/plain; charset=utf-8                                               | 427       |     1 |
| text/xml                                                                | 1334      |     1 |
| text/xml; charset=UTF-8                                                 | 3039189   |   654 |
| video/mp4                                                               | 16785642  |     1 |

### 4. Анализ через *wpull*

`wpull http://velizhnov67.ru/ --strip-session-id --no-check-certificate --no-robots --span-hosts --page-requisites --sitemaps --inet4-only --timeout 20 --tries 3 --waitretry 5 --recursive --level inf --retry-connrefused --retry-dns-error --delete-after --warc-append --warc-cdx -U "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:101.0) Gecko/20100101 Firefox/101.0" -d -a velizhnov67.ru/velizhnov67.ru.log --database velizhnov67.ru/sitearchive-velizhnov67.ru.db --warc-file "velizhnov67.ru/velizhnov67.ru" --warc-header "operator: No Name" --warc-header "downloaded-by: Student"  --domains velizhnov67.ru --concurrent 4`

### 5. Выводы и интерпретации

Как показывают сравнительные таблицы, в структуре сайта содержится больше всего изображений в форматах jpg, jpeg и png, если не включать файлы с пустым расширением.

Самый распространённый тип MIME - изображения в формате jpeg, которые весят больше всех остальных типов файлов вместе взятых. На втором месте стоит тип данных "text/html" в кодировке utf-8; на третьем - "application/json" в кодировке utf-8.

По результатам обработки через ArchiveReady общий коэффициент качества архивации данного сайта составляет 76%; это было обеспечено очень высоким параметром согласованности (Cohesion) соответствию стандартам (Standards Compliance). Однако уровень доступности (Accessibility), который имеет значение 59%, привёл к понижению общей оценки анализа.

Параметр Accesibility имеет значение чуть выше среднего - около 60% метаданных было корректно распознано. Количество выкачанных ссылок и медиафайлов также оказалось низким. Однако количество извлечённых медиафайлов оказалось больше. Поэтому можно сделать вывод, что лишь часть файлов в структуре была успешно проанализирована ArchiveReady.

Полностью выкачать все метаданные не получилось, однако значение держится на приличном уровне (75%). Можно сделать вывод, что имеющихся данных достаточно, чтобы сделать общий вывод о качестве работы анализатора.
