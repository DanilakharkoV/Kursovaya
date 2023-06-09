База данных школы
Эта база данных предназначена для хранения информации, связанной с школой, включая аудитории, группы, студентов, предметы, учителей, уроки и связи между студентами и уроками.

Назначение
Цель этой базы данных - облегчить управление данными, связанными с школой, такими как расписание занятий, запись студентов, назначение учителей и детали уроков. Она позволяет эффективно организовывать и извлекать информацию о различных сущностях в школьной системе.

Технические требования
Для работы с этой базой данных вам потребуется:

Установленный сервер MySQL (совместимая версия с дампом базы данных).
MySQL Workbench или любой другой клиентский инструмент для работы с MySQL.

Начало работы
Скачайте и установите сервер MySQL, если он еще не установлен.

Откройте MySQL Workbench или любой другой клиентский инструмент для работы с MySQL.

Создайте новую схему базы данных с именем "school".

Импортируйте предоставленный дамп базы данных (например, database/school_dump.sql) в схему "school".

После импорта базы данных вы можете выполнять типичные запросы, указанные выше, или выполнять другие операции по необходимости.

Схема базы данных
Схема базы данных включает следующие таблицы:

classroom: Хранит информацию об аудиториях, включая идентификатор, номер и вместимость.
group: Хранит информацию о группах студентов, включая идентификатор, название и связанный курс.
student: Хранит информацию о студентах, включая идентификатор, полное имя, дату рождения и связанную группу.
object: Хранит информацию о предметах, включая идентификатор и название.
teacher: Хранит информацию об учителях, включая идентификатор и полное имя.
object_teacher: Хранит связи между предметами и учителями.
leason: Хранит информацию об уроках, включая идентификатор, дату и время, связанную аудиторию, учителя и предмет.
student_leason: Хранит связи между студентами, уроками и группами студентов.