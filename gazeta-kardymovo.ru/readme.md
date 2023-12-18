## Название сайта: gazeta-kardymovo.ru

### 1. О чём сайт

«ДЕСНА» - газета муниципального образования, которая выпускается в гор. округе Десногорск Смоленской области.

### 2. Характеристики по данным ArchiveReady

![ArchiveReady_Gazeta_Kardymovo](https://github.com/DukeNukem4ever/DemoGit/assets/31654733/542212c2-c567-4aba-a65a-19dace6b2fa4)

### 3. Характеристики по данным *metawarc*

#### 3.1. Код, который был нужен для реализации функций по metawarc

`metawarc metadata gazeta-kardymovo.ru.warc` - извлекает метаданные из ".warc"-файла; возвращает json-строки по каждому найденному файлу.

`metawarc analyze gazeta-kardymovo.ru.warc` - анализ на обнаружение типов данных, соответствующих стандарту MIME.

`metawarc index gazeta-kardymovo.ru.warc` - генерация базы данных с метаданными в формате ".db"

`metawarc export -t content -o content.jsonl gazeta-kardymovo.ru.warc` - экспорт HTML-содержания веб-сайта в формате jsonl.

`metawarc stats -m mimes` - получение информации о частоте типов данных, соответствующих стандарту MIME.

`metawarc stats -m exts` - получение информации о частоте типов расширений данных.

#### 3.2. Сравнительная таблица

##### 3.2.1 Информация по расширениям файлов

| extension | size       | count |
|-----------|------------|-------|
|           | 238747742  | 12629 |
| css       | 181321     |     5 |
| docx      | 430536     |     8 |
| eot       | 317642     |     3 |
| jpeg      | 40195835   |   615 |
| jpg       | 1164539741 | 10875 |
| js        | 197008     |    10 |
| pdf       | 2242365    |     2 |
| php       | 1374       |     2 |
| png       | 69427961   |   223 |
| svg       | 1358886    |     3 |
| ttf       | 317195     |     3 |
| txt       | 426        |     1 |
| woff      | 169945     |     3 |
| woff2     | 138903     |     3 |
| xml       | 15184      |     2 |

##### 3.2.2 Информация по MIME-типам данных

| mime                                                                    | size       | count |
|-------------------------------------------------------------------------|------------|-------|
| application/json; charset=UTF-8                                         | 6083837    |  1792 |
| application/octet-stream                                                | 626043     |     9 |
| application/pdf                                                         | 2242365    |     2 |
| application/rss+xml; charset=UTF-8                                      | 31083777   |  2046 |
| application/vnd.ms-fontobject                                           | 317642     |     3 |
| application/vnd.openxmlformats-officedocument.wordprocessingml.document | 430536     |     8 |
| application/x-javascript                                                | 197008     |    10 |
| image/jpeg                                                              | 1203676891 | 11414 |
| image/png                                                               | 69330569   |   216 |
| image/svg+xml                                                           | 1358886    |     3 |
| text/css                                                                | 181321     |     5 |
| text/html; charset=UTF-8                                                | 196823923  |  7494 |
| text/plain                                                              | 280        |     1 |
| text/plain; charset=utf-8                                               | 426        |     1 |
| text/xml                                                                | 1335       |     1 |
| text/xml; charset=UTF-8                                                 | 5927225    |  1382 |

### 4. Анализ через *wpull*

`wpull http://gazeta-kardymovo.ru/ --strip-session-id --no-check-certificate --no-robots --span-hosts --page-requisites --sitemaps --inet4-only --timeout 20 --tries 3 --waitretry 5 --recursive --level inf --retry-connrefused --retry-dns-error --delete-after --warc-append --warc-cdx -U "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:101.0) Gecko/20100101 Firefox/101.0" -d -a gazeta-kardymovo.ru/gazeta-kardymovo.ru.log --database gazeta-kardymovo.ru/sitearchive-gazeta-kardymovo.ru.db --warc-file "gazeta-kardymovo.ru/gazeta-kardymovo.ru" --warc-header "operator: No Name" --warc-header "downloaded-by: Student"  --domains gazeta-kardymovo.ru --concurrent 4`

### 5. Выводы и интерпретации

Как показывают сравнительные таблицы, в структуре сайта содержится больше всего изображений в форматах jpg, jpeg и png, если не включать файлы с пустым расширением.

Самый распространённый тип MIME - изображения в формате jpeg, которые весят больше всех остальных типов файлов вместе взятых. На втором месте стоит тип данных "text/html" в формате utf-8.

По результатам обработки через ArchiveReady общий коэффициент качества архивации данного сайта составляет 76%; это было обеспечено очень высоким параметром согласованности (Cohesion) соответствию стандартам (Standards Compliance). Однако уровень доступности (Accessibility) равняется 53%, из-за чего итоговая оценка значительно ухудшилась.

Параметр Accesibility имеет весьма низкое значение - это говорит о том, что чуть больше половины метаданных было корректно распознано. Количество выкачанных ссылок и медиафайлов также оказалось низким; из-за чего можно сделать вывод о том, что некоторые файлы не поддаются анализу через ArchiveReady.

Полностью выкачать все метаданные не получилось, поэтому взаимодействие сервиса с контентом не является идеальным. Тем не менее, значение держится на хорошем уровне (80%), и это обеспечивает адекватный анализ полученных данных.
