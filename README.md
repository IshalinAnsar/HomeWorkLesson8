# HomeWorkLesson8
На семинаре:

Создать телефонный справочник с возможностью импорта и экспорта данных в формате .txt. Фамилия, имя, отчество, номер телефона - данные, которые должны находиться в файле.

Так же на семинаре:
Программа должна выводить данные.
Программа должна сохранять данные в текстовом файле.
Пользователь может ввести одну из характеристик для поиска определенной записи(Например имя или фамилию человека).

Задача:
Дополнить справочник возможностью копирования данных из одного файла в другой. Пользователь вводит номер строки, которую необходимо перенести из одного файла в другой.

Решение задачи:
При запуске программа предлагает создать новый список номеров или сгенерировать список случайных номеров, а также открыть существующий список номеров.

Создание списка номеров
В режиме создания списка номеров программа предлагает ввести имя файла для новой таблицы, сохраняет файл с шапкой новой таблицы и переходит в режим работы с открытым файлом.

Генерация списка случайных номеров
В режиме генерации списка случайных номеров программа запрашивает параметры списка: количество записей и имя файла для сохранения. После генерации списка выводит его в консоль и переходит в режим работы с открытым файлом.

Открытие файла
В режиме открытия существующего файла программа сканирует директорию, из которой запускается, на предмет наличия в ней таблиц .csv.

Программа выводит на экран список таблиц и предлагает выбрать таблицу для дальнейшей работы, после чего переходит в режим работы с открытым файлом.

Режим работы с открытым файлом
В режиме работы с открытым файлом можно использовать следующие команды:

"a" для добавления контакта
"d" для удаления контакта по его порядковому номеру
"e" для редактирования контакта
"f" для поиска контакта
"m" для переноса (экспорта) контакта в другой файл
"s" для сохранения файла
"sa" для сохранения файла под другим именем
"b" для возврата в главное меню
Для создания нового номера телефона программа последовательно запрашивает имя, отчество, фамилию, номер телефона.

Номер телефона проверяется по формату, прочие поля могут принимать любые, в т.ч. пустые значения.

Особенности поиска контактов
Для поиска контактов поисковый запрос переводится в нижний регистр, разбивается на слова по пробелам. Для каждого контакта проверяется наличие слов поискового запроса в каждом из полей. Каждое совпадение дает контакту 1 очко. После того, как все контакты проверены, контакты, имеющие хотя бы одно очко, сортируются в порядке убывания количества очков (в порядке возрастания индекса для контактов с одинаковым количеством очков) и выводятся в консоль.
