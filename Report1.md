# Отчет о тестировании Инструкции по установке OpenJDK11 #

## Краткое описание ##

12.03.2021 г. было проведено Функциональное тестирование инструкции по установке OpenJDK11.

На тестирование затрачено: *1 час*

В результате тестирования выявлены следующие дефекты:
*не выявлены*

## Описание процесса тестирования ##

В процессе тестирования использовались следующие артефакты:
*Инструкция по установке OpenJDK 11*

## Перечисление данных с ожидаемым результатом: ##

1. ### Шаг ### 

Перейти на сайт adoptopenjdk.net. 

* Ожидаемый результат (ОР):

Осуществляется переход на сайт adoptopenjdk.net*

* Фактический результат:

Соответствует ОР.
Осуществляется переход на сайт adoptopenjdk.net

[Приложение](https://adoptopenjdk.net/) 

2. ### Шаг ### 

Выбрать опцию как на скриншоте (см. “Приложения”) и нажать на кнопку скачивания

* Ожидаемый результат (ОР):

Опции выбираются, кнопка для скачивания запускает процесс установки PKG-файла

* Фактический результат:

Соответствует ОР

[Приложение](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/pic/mac-adoptopenjdk.png)


3. ### Шаг ###

Запустить на установку скачанный PKG-файл и нажать кнопку "Продолжить"

* Ожидаемый результат (ОР):

Запускается установочный модуль ПО, закладка - “Введение”,
кнопка “Продолжить” открывает лицензионное соглашение (закладка - “Лицензия”)

* Фактический результат:

Соответствует ОР


[Приложение](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/pic/mac-step1.png)


4. ### Шаг ###

Подтверждение ознакомления с условиями лицензии

* Ожидаемый результат (ОР):

В установочном модуле открывается лицензионное соглашение (ЛС) для ознакомления; 
кнопка “Напечатать” - запускает ЛС на печать, кнопка “Сохранить” - сохраняет текстовый файл ЛС, 
кнопка “Назад” - возвращает пользователя на предыдущую закладку “Введение” установочного модуля (см. шаг 3),
кнопка “Продолжить” - переключает на закладку - “Размещение”

* Фактический результат:

Соответствует ОР


[Приложение](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/pic/mac-step2.png)


5. ### Шаг ###

Выбор диска для установки

* Ожидаемый результат (ОР):

В установочном модуле открывается закладка - “Размещение”;
кнопка “Назад” - возвращает пользователя на предыдущую закладку “Лицензионное соглашение” установочного модуля (см. шаг 4),
кнопка “Продолжить” - переключает на закладку - “Тип установки”

* Фактический результат:

Соответствует ОР


[Приложение](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/pic/mac-step4.png) 


6. ### Шаг ###

Установка ПО

* Ожидаемый результат (ОР):

В установочном модуле открывается закладка - “Тип установки”;
кнопка “Назад” - возвращает пользователя на предыдущую закладку “Тип установки” см. шаг 5), 
кнопка “Установить” - запускает процесс установки ПО

* Фактический результат:

Соответствует ОР


[Приложение](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/pic/mac-step4.png)


7. ### Шаг ###

Завершение установки ПО

* Ожидаемый результат (ОР):

После завершения установки ПО - в установочном модуле открывается вкладка “Обзор”
клавиша “Назад” - не активна,
клавиша “Закрыть” - закрывает установочный модуль.
После завершения установки ПО - в установочном модуле открывается вкладка “Обзор”
клавиша “Назад” - не активна,
клавиша “Закрыть” - закрывает установочный модуль.

* Фактический результат:

Соответствует ОР


[Приложение](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/pic/mac-step5.png) 

8. ### Шаг ###

Проверка установленного ПО
Запустить терминал.

В командной строке ввести <java -version>

* Ожидаемый результат (ОР):

Терминал выводит сообщение:
"openjdk version "11.0.5" 2019-10-15
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.5+10)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.5+10, mixed mode)"

* Фактический результат:

Соответствует ОР

Примечание: *открывать терминал только после установки ПО*


### В качестве тестовых данных использовались данные: ###

[Приложение](https://adoptopenjdk.net/)

### Тестирование производилось в следующем окружении: ###

macOS Catalina версия 10.15.7
Google Chrome версия 88.0.4324.192 (Официальная сборка), (x86_64)
