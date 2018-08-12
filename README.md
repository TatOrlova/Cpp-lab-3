

<img src="img/green.png" width="50" height="50">

# Cpp-lab-3

## Задачи для практикума №3 (классы)

### Задача


> Разработать систему классов для программы имитационного моделирования "Океан". Моделируется замкнутая экологическая система по принципу хищник-жертва.

### Описание системы

В системе рассматриваются сущности:

- **Ocean** - двумерная матрица ячеек.
- **Cell** - ячейка океана, которая может быть либо пустой, либо содержать объект.
- **Object** - базовый класс для объектов, прикрепленных к ячейке.
- **Stone** - неподвижный объект океана, просто занимающий ячейку.
- **Coral** - неподвижный объект, растущий от центральной ячейки равномерно во все стороны.
- **Prey** - рыба-жертва. Передвигается случайным образом по океану, размножается и умирает через заданные промежутки времени.
- **Predator** - рыба-хищник. Передвигается по океану, поедает рыбу-жертву, размножается. Может умереть от голода.

### Параметры

Каждый объект содержит ряд параметров, от которых зависит процесс моделирования

1. **Ocean**
  - размер по горизонтали и вертикали
1. **Coral**
  - время цикла размножения
1. **Prey**
  - время жизни
  - время цикла размножения
1. **Predator**
  - время жизни
  - время цикла размножения
  - время цикла питания

Данные параметры должны задаваться в текстовом файле любого формата (txt,xml,json)  и использоваться при инициализации океана.

### Консольная версия

Программа должна выводить на консоль состояние океана в определенные моменты времени (итерации). Каждый объект в океане имеет определенный символ для отображения на экране.

Примерный вид океана:

<img src="img/ocean.png" width="550" height="350">

### Выполнение программы

В начале программы происходит инициализация океана, в него помещается заданное число объектов, а потом запускается процесс имитации. Имитация состоит из отдельных шагов (итераций). Заканчивается процесс при наступлении одного из следующих событий:

- пользователь прерывает выполнение программы;
- в океане не осталось ни одного живого объекта;
- в океане остался только один вид живых обектов.

### Тестирование

Для программы необходимо разработать набор модульных тестов и поместить их в файл `tests.cpp`. Тесты должны покрывать основной функционал программы.
  
 
## Список участников/веток

|  ФИО              | Имя ветки |
|-------------------|-----------|
| Алексеева В.     | b1 |
| Белов А.     | b2 |
| Булатова М.    | b3 |
| Зобов М.|  b4 |
| Зубова М.         | b5  |
| Исхаков М.        | b6 |
| Косолапов В.       | b7 |
| Котрикова К.     | b8 |
| Коченко А.       | b9 |
| Макаров Д.     | b10 |
| Михайлова И.           | b11 |
| Орлова Т.   | b12  |
| Парьев Д.      | b13 |
| Першина А.        | b14 |
| Решетников Н.            | b15 |
| Семенов А. | b16 |
| Серов Д.      | b17 |
| Смирнова М. | b18 |
| Сорокин А.  | b19 |
| Тимофеев С.   | b20 |
| Тюлькин А.     | b21 |
| Федяков М.   |  b22 |
| Яковлев Д.   | b23 |

## Алгоритм выполнения работы

Для выполнения работы необходимо:

1. Выполнить *fork* репозитария в свой аккаунт.
1. Выполнить клонирование репозитария из своего аккаунта к себе на локальную машину (`git clone`).
1. Создать ветку **git** с индивидуальным номером (`git branch имя_ветки`).
1. Сделать ветку активной (`git checkout имя`).
1. Необходимо разместить как исходные файлы с решениями задач, поместив **cpp** файлы в **src**, а заголовочные - в **include**. 
1. Добавить файлы в хранилище (`git add`).
1. Выполнить фиксацию изменений (`git commit -m "комментарий"`).
1. Отправить содержимое ветки в свой удаленный репозитарий (`git push origin имя_ветки`).
1. Создать пул-запрос в репозитарий группы и ждать результата от **Travis-CI**.

