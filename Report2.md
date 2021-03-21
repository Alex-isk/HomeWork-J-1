# Отчет о тестировании Руководства использования KeyValidator #

## Краткое описание ##

12.03.2021 г. было проведено Функциональное тестирование руководства использования KeyValidator.

На тестирование затрачено: *1 час*

## В результате тестирования выявлены следующие дефекты: ##

#### Из 5 представленных валидных ключей выявлено 2 *невалидных* ключа: ####
[Bag-report-task2](https://github.com/Alex-isk/HomeWork-J-1/issues/1)

#### Из 5 представленных невалидных ключей выявлен 1 валидный ключ: ####

[Bag-report-task2](https://github.com/Alex-isk/HomeWork-J-1/issues/1)


## Описание процесса тестирования ##

В процессе тестирования использовались следующие артефакты:
 
*Руководство использования KeyValidator*

В качестве тестовых данных использовались данные:

[Ключи для проверки](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md#%D0%BA%D0%BB%D1%8E%D1%87%D0%B8-%D0%B4%D0%BB%D1%8F-%D0%BF%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B8)


## Перечисление данных с ожидаемым результатом: ##

1. ### Шаг ### 

Скачать файл [KeyValidator.class](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/artifacts/KeyValidator.class) в локальную папку. По адресу папки открыть терминал.

2. ### Шаг ### 

Ввести в терминал следующие данные (валидных ключей):

java KeyValidator 8f05e6a7-70e9-33d7-bfe7-b19eae0d899 80b427f8-92cd-3aae-ba04-3927fbe17c6 b295bc63-9f03-3b4b-af80-969b39f8c262 387eedc6-12e9-3b32-9881-63b6b5e85317 c19a8cf9-5c3a-37c5-b7f3-d16d38a0c18

* Ожидаемый результат (ОР):

Result for 8f05e6a7-70e9-33d7-bfe7-0b19eae0d899: OK

Result for 80b427f8-92cd-3aae-ba04-03927fbe17c6: OK

Result for b295bc63-9f03-3b4b-af80-969b39f8c262: OK

Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: OK

Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: OK

* Фактический результат:

Не соответствует ОР

[Bag-report-task2](https://github.com/Alex-isk/HomeWork-J-1/issues/1)

3. ### Шаг ### 

Ввести в терминал следующие данные (невалидных ключей):

java KeyValidator 18252235-78e0-44a5-8720-556f0c7da17a  e66075b6-ddad-445e-baf6-161b3289522b b6d53250-f07e-4352-a293-6102ddf7f1ca c2bc778a-1cb9-46c6-b435-0489649d2a42 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1


* Ожидаемый результат (ОР):

Result for 8f05e6a7-70e9-33d7-bfe7-0b19eae0d899: *FAIL*

Result for 80b427f8-92cd-3aae-ba04-03927fbe17c6: *FAIL*

Result for b295bc63-9f03-3b4b-af80-969b39f8c262: *FAIL*

Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: *FAIL*

Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: *FAIL*

* Фактический результат:

Не соответствует ОР

[Bag-report-task2](https://github.com/Alex-isk/HomeWork-J-1/issues/1)

### Тестирование производилось в следующем окружении: ###

macOS Catalina версия 10.15.7
Google Chrome версия 88.0.4324.192 (Официальная сборка), (x86_64)
