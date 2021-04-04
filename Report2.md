# Отчет о тестировании Credit Card Number Validator #

## Краткое описание ##

12.03.2021 г. было проведено Функциональное тестирование ПО Credit Card Number Validator.

На тестирование затрачено: *1 час*

## В результате тестирования дефекты не выявлены: ##


## Описание процесса тестирования ##

### В процессе тестирования использовались следующие артефакты: ###

* *IntelliJ IDEA 2020.3.2 (Community Edition)*
 
* *программный код Credit Card Number Validator:*


```
  public class Main {
  public static void main(String[] args) {
    // TODO: подставлять номер карты нужно сюда между двойными кавычками, без пробелов
    String number = "5351719427810741";
    System.out.println(String.format("Result is %s", isValidCardNumber(number) ? "OK" : "FAIL"));
  }

  public static boolean isValidCardNumber(String number) {
    if (number == null) {
      return false;
    }

    if (number.length() != 16) {
      return false;
    }

    long result = 0;
    for (int i = 0; i < number.length(); i++) {
      int digit;
      try {
        digit = Integer.parseInt(number.charAt(i) + "");
      } catch (NumberFormatException e) {
        return false;
      }

      if (i % 2 == 0) {
        digit *= 2;
        if (digit > 9) {
          digit -= 9;
        }
      }
      result += digit;
    }

    return (result != 0) && (result % 10 == 0);
  }
}
```


### В качестве тестовых использовались данных банковских карт: ###

[Тестовые банковские карты](https://www.freeformatter.com/credit-card-number-generator-validator.html)


## Перечисление данных с ожидаемым результатом: ##

1. ### Шаг ### 

* Запустить IntelliJ IDEA
* Создать метод Main
* Вставить программый код Credit Card Number Validator

2. ### Шаг ### 

Запустить программый код Credit Card Number Validator в IntelliJ IDEA
с валидными номерами банковских карт: 
* 4556169122823589
* 2720996481143208


### Ожидаемый результат (ОР): ###

Result is OK

### Фактический результат - соответствует ОР ### 

Скриншот результата проверки валидной банковской карты 4556169122823589![image](https://user-images.githubusercontent.com/79845756/112984670-dbc96500-9167-11eb-995f-155ea32ec328.png)


Скриншот результата проверки валидной банковской карты 2720996481143208![image](https://user-images.githubusercontent.com/79845756/112984856-16cb9880-9168-11eb-9a6f-de4149d83370.png)


3. ### Шаг ### 

Запустить программый код Credit Card Number Validator в IntelliJ IDEA
с невалидными номерами банковских карт: 
* 4929736236978000
* 2770996481143208


### Ожидаемый результат (ОР): ###

Result is FAIL

### Фактический результат - соответствует ОР ###

Скриншот результата проверки невалидной банковской карты 4929736236978000![image](https://user-images.githubusercontent.com/79845756/112985924-84c48f80-9169-11eb-9895-a5fd555bcf53.png)



Скриншот результата проверки невалидной банковской карты 2770996481143208![image](https://user-images.githubusercontent.com/79845756/112986005-a02f9a80-9169-11eb-88ba-88af25b06ffd.png)





### Тестирование производилось в следующем окружении: ###

macOS Catalina версия 10.15.7

IntelliJ IDEA 2020.3.2 (Community Edition) 
Версия среды выполнения: 11.0.9.1 + 11-b1145.77 
x86_64 VM: 64-разрядная серверная виртуальная машина OpenJDK от JetBrains sro

