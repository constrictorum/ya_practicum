# Проект "Поиск изображений по описаниям"

## Данные

В файле `train_dataset.csv` находится информация, необходимая для обучения: имя файла изображения, идентификатор описания и текст описания. Для одной картинки может быть доступно до 5 описаний. Идентификатор описания имеет формат <имя файла изображения>#<порядковый номер описания>.

В папке `train_images` содержатся изображения для тренировки модели.

В файле `CrowdAnnotations.tsv`  — данные по соответствию изображения и описания, полученные с помощью краудсорсинга. Номера колонок и соответствующий тип данных:
1. Имя файла изображения.
1. Идентификатор описания.
1. Доля людей, подтвердивших, что описание соответствует изображению.
1. Количество человек, подтвердивших, что описание соответствует изображению.
1. Количество человек, подтвердивших, что описание не соответствует изображению.

В файле `ExpertAnnotations.tsv`  — данные по соответствию изображения и описания, полученные в результате опроса экспертов. Номера колонок и соответствующий тип данных:
1.    Имя файла изображения.
1.    Идентификатор описания.

3, 4, 5 — оценки трёх экспертов. 

Эксперты ставят оценки по шкале от 1 до 4, где 1 — изображение и запрос совершенно не соответствуют друг другу, 2 — запрос содержит элементы описания изображения, но в целом запрос тексту не соответствует, 3 — запрос и текст соответствуют с точностью до некоторых деталей, 4 — запрос и текст соответствуют полностью.      

В файле `test_queries.csv` находится информация, необходимая для тестирования: идентификатор запроса, текст запроса и релевантное изображение. Для одной картинки может быть доступно до 5 описаний. Идентификатор описания имеет формат <имя файла изображения>#<порядковый номер описания>.

В папке `test_images` содержатся изображения для тестирования модели.

## Задача

Постройте модель, которая епринимает на вход описание в свободной форме и возвращает список изображений из библиотеки, наиболее соответствующих описанию.

## Используемые библиотеки
*pandas*,  *nltk*, *tensorflow*, *sklearn*, *PIL*