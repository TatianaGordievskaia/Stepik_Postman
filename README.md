# Stepik_Postman
Курс "Тестирование ПО: Postman для тестирования API"

![](https://github.com/TatianaGordievskaia/Stepik_Postman/blob/main/stepik-certificate.png)


1. Какие типы запросов можно отправлять с помощью Postman?
 - [ ] SQL запросы
 - [X] Запросы к REST и SOAP API
 - [ ] Запросы к NOSQL базам данных
 - [X] GraphQL запросы
2. Можно ли с помощью Postman отправлять HTTP запросы?
- [ ] Нет
- [X] Да
3. Можно ли с помощью Postman отправлять HTTPS запросы?
- [X] Да
- [ ] Нет
4. Какой тип запроса обычно используется для чтения информации?
- [ ] PATCH
- [X] GET
- [ ] PUT
- [ ] POST
5. Какие типы запросов обычно используется для обновления информации?
- [X] PATCH
- [ ] DELETE
- [ ] POST
- [X] PUT
- [ ] GET
6. У нас есть запрос, содержащий path параметр : https://postman-echo.com/book/{id}/get

Как будет выглядеть его вызов в Postman, если мы хотим передать значение id, на вкладке Params?
- [ ] https://postman-echo.com/book/{id}/get
- [X] https://postman-echo.com/book/:id/get
- [ ] https://postman-echo.com/book/id/get
- [ ] https://postman-echo.com/book/10/get
7. У нас есть GET запрос с двумя query параметрами : https://postman-echo.com/get?param1=value1&param2=value2

Как эти параметры будут выглядеть в bulk edit, на вкладке Params?
```
 param1:value1
 param2:value2
 ```
8. Вы хотите отправить POST запрос. В теле запроса содержатся данные в формате XML.

Какой формат вам нужно выбрать на вкладке Body?
- [ ] form-data
- [X] raw
- [ ] none
- [ ] binary
9. Вы хотите отправить DELETE запрос с пустым телом. Какой формат вам нужно выбрать на вкладке Body?
- [ ] raw
- [ ] x-www-form-urlencoded
- [X] none
- [ ] binary
10. Вы хотите отправить POST запрос. В теле запроса хотите передать картинку.

Какой формат вам нужно выбрать на вкладке Body?
- [X] binary
- [ ] raw
- [ ] GraphQL
- [ ] none
11. В теле ответа нам пришёл json объект. На какой вкладке удобнее посмотреть его содержимое?
- [ ] Raw
- [X] Pretty
- [ ] Preview
12. В теле ответа нам пришла стандартная ошибка в виде html файла. На какой вкладке будет удобнее посмотреть ее содержимое?
- [ ] Pretty
- [ ] Raw
- [X] Preview
13. Какая информация об ответе доступна в Postman?
- [X] Время ответа от сервера
- [X] Код ответа
- [X] Размер ответа
14. Какое из определений больше всего подходит для коллекции?
- [ ] Представляет собой набор переменных.
- [X] Позволяет группировать различные запросы.
- [ ] Позволяет хранить и повторно использовать различные значения.
15. Можно ли добавить глобальную переменную и переменную уровня коллекции с одинаковым именем?
- [ ] Нет
- [X] Да
16. Переменная с именем param определена на трех уровнях. Она имеет следующие значения:

На уровне окружения local, переменная param = env.
Глобальная переменная param = global.
На уровне коллекции, переменная param = collection.
Внутри коллекции мы создали новый запрос : 

https://postman-echo.com/get?param={{param}}

С каким значением параметра param выполнится запрос, если у нас выбрано окружение local.
```
 env
 ```
17. Переменная с именем param определена на трех уровнях. Она имеет следующие значения:

На уровне окружения local, переменная param = env.
Глобальная переменная param = global.
На уровне коллекции, переменная param = collection.
Внутри коллекции мы создали новый запрос : 

https://postman-echo.com/get?param={{param}}

С каким значением выполнится запрос, если у нас не выбрано окружение.
```
collection
```
18. Какое из определений больше всего подходит для переменной?
- [ ] Представляет собой набор переменных.
- [ ] Позволяет группировать различные запросы.
- [X] Позволяет хранить и повторно использовать различные значения.
19. Какое из определений больше всего подходит для окружения?
- [ ] Позволяет хранить и повторно использовать различные значения.
- [X] Представляет собой набор переменных.
- [ ] Позволяет группировать различные запросы.
20. Расставьте следующие действия в порядке, в котором их запускает Postman.
> Запуск pre-request скрипта
> Отправка запроса

> Получение ответа

> Запуск тестового скрипта
21. Расставьте следующие действия в порядке их запуска.
> Pre-request скрипт на уровне коллекции

> Pre-request скрипт на уровне папки

> Pre-request скрипт на уровне запроса

> Тестовый скрипт на уровне коллекции

> Тестовый скрипт на уровне папки

> Тестовый скрипт на уровне запроса
22. У нас есть глобальная переменная param = global. Будем использовать ее в запросе:

https://postman-echo.com/get?name={{param}}

У запроса на вкладке pre-request script добавим такой код:
```
pm.variables.set("param", "other");
```
После нажатия на кнопку Send, с каким значением параметра name будет выполнен запрос?
- [ ] "name"
- [ ] "global"
- [X] "other"
- [ ] "param"
23. У нас есть глобальная переменная param = global. Будем использовать ее в запросе:

https://postman-echo.com/get?name={{param}}

У запроса на вкладке test script добавим такой код:
```
pm.variables.set("param", "test");
```
После нажатия на кнопку Send, с каким значением параметра name будет выполнен запрос?
- [ ] "name"
- [ ] "param"
- [ ] "test"
- [X] "global"
24. У нас есть переменная timer. В глобальных переменных она имеет значение равное 10. В коллекции Lesson_5 ее значение = 5. В окружении Local она имеет значение равное 2. В коллекции Lesson_5 есть запрос. На вкладке pre-request у него добавлен код:
```
console.log(pm.variables.get("timer"));
```
Если отправить запрос, выбрав в списке окружений "No Environment", что будет выведено в консоли?
```
5
```
25. У нас есть переменная count. В глобальных переменных она имеет значение равное 10. В коллекции Lesson_5 ее значение = 5. В окружении Local она не определена. В коллекции Lesson_5 есть запрос. На вкладке pre-request у него добавлен код:
```
console.log(pm.environment.get("count"));
```
Если отправить запрос, выбрав в списке окружений "Local", что будет выведено в консоли?
```
undefined
```
26. У нас есть запрос, содержащий два query параметра:

POST https://postman-echo.com/post?param1=value&param2=value

На вкладке pre-request мы добавили следующий код:
```
pm.request.removeQueryParams("value");
```
Нажав кнопку Send, какие query параметры мы отправим в запросе?
- [X] param1=value и param2=value
- [ ] никаких
- [ ] param2=value
- [ ] param1=value
27. Ответ от сервера выглядит следующим образом:
![](https://github.com/TatianaGordievskaia/Stepik_Postman/blob/main/05_4_1.png)
На вкладке Tests добавлен такой код:
```
console.log(pm.response.status);
```
Что будет выведено в консоли,  после получения ответа от сервера?
- [ ] ничего
- [ ] 200 OK
- [X] OK
- [ ] 200

