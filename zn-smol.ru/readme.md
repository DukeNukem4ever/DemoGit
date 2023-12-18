## Название сайта: zn-smol.ru

### 1. О чём сайт

"Знамя" - общественно-политическая газета Ельнинского района Смоленской области.

### 2. Характеристики по данным *ArchiveReady*
![ArchiveReady_Zn_Smol](https://github.com/DukeNukem4ever/DemoGit/assets/31654733/9e5d0f16-7a5e-4cb1-b34a-069d2ab8fa02)

### 3. Характеристики по *metawarc*

#### 3.1. Код, который был нужен для реализации функций по *metawarc*

`metawarc metadata zn-smol.ru.warc` - извлекает метаданные из ".warc"-файла; возвращает json-строки по каждому найденному файлу.

`metawarc analyze zn-smol.ru.warc` - анализ на обнаружение типов данных, соответствующих стандарту MIME.

`metawarc index zn-smol.ru.warc` - генерация базы данных с метаданными в формате ".db"

`metawarc export -t content -o content.jsonl zn-smol.ru.warc` - экспорт HTML-содержания веб-сайта в формате jsonl.

`metawarc stats -m mimes` - получение информации о частоте типов данных, соответствующих стандарту MIME.

`metawarc stats -m exts` - получение информации о частоте типов расширений данных.

#### 3.2. Сравнительная таблица

##### 3.2.1 Информация по расширениям файлов

| extension | size      | count |
|-----------|-----------|-------|
|           | 180867699 |  4851 |
| css       | 124363    |    10 |
| eot       | 374736    |     4 |
| gif       | 1619446   |    11 |
| ico       | 1528      |     1 |
| jpeg      | 11186526  |   107 |
| jpg       | 952026055 |  4881 |
| js        | 318032    |    22 |
| png       | 25286254  |    62 |
| rar       | 370104807 |    51 |
| ru        | 382       |     1 |
| svg       | 1961457   |     8 |
| ttf       | 373930    |     4 |
| txt       | 883       |     2 |
| woff      | 210801    |     4 |
| woff2     | 169364    |     3 |
| xml       | 466017    |     5 |
| zip       | 412813524 |    36 |


##### 3.2.2 Информация по MIME-типам данных

| mime                          | size      | count |
|-------------------------------|-----------|-------|
| application/javascript        | 318032    |    22 |
| application/json              | 1710      |     5 |
| application/octet-stream      | 14651315  |    87 |
| application/vnd.ms-fontobject | 374736    |     4 |
| application/x-rar-compressed  | 370104513 |    50 |
| application/zip               | 412813230 |    35 |
| font/woff                     | 210801    |     4 |
| font/woff2                    | 169364    |     3 |
| image/gif                     | 1613977   |     9 |
| image/jpeg                    | 949548065 |  4852 |
| image/png                     | 24661802  |    59 |
| image/svg+xml                 | 1961457   |     8 |
| image/x-icon                  | 1528      |     1 |
| text/css                      | 123775    |     8 |
| text/css;;charset=UTF-8       | 57288     |     3 |
| text/html                     | 704899    |  1879 |
| text/html; charset=UTF-8      | 180118785 |  3020 |
| text/html; charset=iso-8859-1 | 3752      |     9 |
| text/plain                    | 524       |     1 |
| text/xml                      | 465363    |     3 |
| text/xml;charset=utf-8        | 888       |     1 |

### 4. Анализ через *wpull*

`wpull http://zn-smol.ru/ --strip-session-id --no-check-certificate --no-robots --span-hosts --page-requisites --sitemaps --inet4-only --timeout 20 --tries 3 --waitretry 5 --recursive --level inf --retry-connrefused --retry-dns-error --delete-after --warc-append --warc-cdx -U "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:101.0) Gecko/20100101 Firefox/101.0" -d -a zn-smol.ru/zn-smol.ru.log --database zn-smol.ru/sitearchive-zn-smol.ru.db --warc-file "zn-smol.ru/zn-smol.ru" --warc-header "operator: No Name" --warc-header "downloaded-by: Student"  --domains zn-smol.ru --concurrent 4`

### 5. Выводы и интерпретации

Как показывают сравнительные таблицы, в структуре сайта содержится очень много файлов формата jpg; на втором месте стоят файлы jpeg; если не считать пустых файлов. Если рассматривать MIME-типы данных, то среди них по количеству употребления лидируют изображения в формате jpeg; на втором месте идут тексты html с кодировкой utf-8.

Данный сайт не получилось обработать через ArchiveReady; поэтому о качестве извлечённых метаданных ничего нельзя сказать. Тем не менее, это только больше подчёркивает необходимость включения данного вебсайта в коллекцию.
