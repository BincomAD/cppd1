# Домашнее задание 1
В домашнем задании необходимо написать код программы, выполняющую определенную задачу в зависимости от варианта<br/>
Вариант #9<br/>
Необходимо разработать программу, которая обрабатывает данные онлайн сервиса MusicBrainz.<br/>
Датасет можно скачать на официальном сайте MusicBrainz https://data.metabrainz.org/pub/musicbrainz/data/fullexport/<br/>
Необходимый файл mbdump.tar.bz2.<br/>
Описание датасета находится по ссылке https://musicbrainz.org/doc/MusicBrainz_Database/Schema<br/>
Например, для Артиста диаграмма находится по ссылке https://wiki.musicbrainz.org/images/7/7e/artist_entity_details.svg<br/>
Файл датасета представляет из себя сжатый архив из множества текстовых файлов, где данные располагаются в строчках, а поля разделены символом табуляции \t<br/>
Каждая таблица на схемах представлена отдельным файлом с аналогичным названием<br/>

Скачать датасет по ссылке можно с помощью команды wget, например
wget https://data.metabrainz.org/pub/musicbrainz/data/fullexport/20230304-002037/mbdump.tar.bz2<br/>
Полученный файл нужно распаковать
tar xvf mbdump.tar.bz2<br/>
Все файлы кроме gender, area, artist, artist_type можно удалить с помощью команды rm.
Программа должна принимать необходимые для работы имена распакованных файлов в качестве аргументов командной строки и выводить данные в стандартный вывод.<br/>
Программа не должна использовать интерактивный ввод с клавиатуры, например, "введите имя файла", "введите необходимый год", "ведите q чтобы выйти" - такими программами не удобно пользоваться и их разработка занимает больше времени.<br/>

Ваш вариант:<br/>
Вывести названия (при наличии) всех групп, которые были основаны в период между двумя годами, переданными в аргументах командной строки
