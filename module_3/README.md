module_3

Проект 3 "О вкусной и здоровой пище"

Задача: подготовка данных для обучения модели, оценивающей рейтинги ресторанов

Исходные данные: файл "main_task.csv", содержащий информацию о ресторанах

Внешний источник: файл "europe_countries_info.py", содержащий информацию о городах и странах Европы (взят с GitHub, доработан под проект)

Что сделано:

1. В исходный датафрейм, содержащий десять признаков, добавлены следующие столбцы (признаки):
 - признак наличия или отсутствия отзывов
 - интервал дат между отзывами
 - является ли город столицей государства
 - в какой стране находится город
 - признак региона: Западная, Восточная, Южная или Северная Европа
 - максимальное значение городского рейтинга в данном городе
 - целочисленное значение признака "id_ta"
 - целочисленное значение признака "restaurant_id"

2. Проведена "оцифровка" следующих признаков:
 - стилей кухни
 - городов
 - стран
 - регионов
 - ценового диапазона

3. Получено значение MAE = 0.18631100884098342

4. Целочисленный признак, выделенный из признака "restaurant_id", на 100% коррелирует с признаком "ranking"

5. Целочисленный признак, выделенный из признака "id_ta", несколько ухудшает показатель МАЕ, поэтому исключён из состава данных