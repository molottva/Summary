## Перечень автоматизируемых сценариев

**Предусловия к сценариям тестирования UI:**

1. Навигация с [главной страницы](https://netology.ru/) на [страницу формы](https://netology.ru/programs/qa) заявки на курс "Тестировщик" через [каталог курсов раздел "Программирование"](https://netology.ru/development) с проверкой фильтрации по курсам
	 ![](./pic/1.png)
	 ![](./pic/2.png)
1. Навигация с [главной страницы](https://netology.ru/) на [страницу формы](https://netology.ru/programs/qa) заявки на курс "Тестировщик" через ["Каталог курсов"](https://netology.ru/navigation) с проверкой фильтрации по курсам
	 ![](./pic/3.png)
	 ![](./pic/4.png)
1. Навигация с [главной страницы](https://netology.ru/) на страницу [каталога курсов раздела "Программирование"](https://netology.ru/development) через [раздел "Направления обучения"](https://netology.ru/#/directions) 
	 ![](./pic/5.png)
1. Навигация с [главной страницы](https://netology.ru/) на страницу [каталога курсов раздела "Программирование"](https://netology.ru/development) через [раздел "Раскройте свои сильные стороны"](https://netology.ru/#/steps) 
	 ![](./pic/6.png)
1. Навигация с [главной страницы](https://netology.ru/) на [страницу формы](https://netology.ru/programs/qa) заявки на курс "Тестировщик" через [раздел "Студенты"](https://netology.ru/#/students)
	 ![](./pic/7.png)
 1. Навигация с футера [главной страницы](https://netology.ru/) на страницу ["Каталог курсов"](https://netology.ru/navigation)
	 ![](./pic/8.png)
1. Навигация с футера [главной страницы](https://netology.ru/) на страницу ["Популярные курсы"](https://netology.ru/popular)
	![](./pic/9.png)
 1. Навигация с футера [главной страницы](https://netology.ru/) на страницу [каталога курсов раздела "Программирование"](https://netology.ru/development)
	 ![](./pic/10.png)
 1. Навигация с [главной страницы](https://netology.ru/) на [страницу формы](https://netology.ru/programs/qa) заявки на курс "Тестировщик" через [рекламное предложение на главной](https://netology.ru/development) с проверкой фильтрации по курсам
	 ![](./pic/11.png)
	 ![](./pic/12.png)
 1. Переход сверху [страницы курса "Тестировщик ПО"](https://netology.ru/programs/qa#/) к [форме записи](https://netology.ru/programs/qa#/order) на курс
	 ![](./pic/13.png)
 1. Проверка появление кнопки "Записаться" и перехода по ней с header [страницы курса "Тестировщик ПО"](https://netology.ru/programs/qa#/) к [форме записи](https://netology.ru/programs/qa#/order) на курс
	 ![](./pic/14.png)
<a/>

**Сценарии тестирования UI:**

1. Успешная отправка валидно* заполненной [формы записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО", включая проверку ввода действующего промокода (с изменением стоимости курса) и перехода на страницы с условиями [политики](https://netology.ru/legal/11)  и  [пользовательского соглашения](https://netology.ru/legal/6)
2. Появление сообщения "Должно состоять из букв" у поля "Имя" при заполнение его спецсимволами в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
3. Появление сообщения "Должно состоять из букв" у поля "Имя" при заполнение его цифрами в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
4. Появление сообщения "Должно быть не короче 2 символов" у поля "Имя" при заполнение его одной буквой в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
5. Появление сообщения "Обязательное поле" у поля "Имя" при оставление поля пустым в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
6. Появление сообщения "Номер в формате +9 (999) 999-99-99" у поля "Телефон" при заполнение поля 8 цифрами в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
7. Появление сообщения "Номер в формате +9 (999) 999-99-99" у поля "Телефон" при заполнение поля 15 цифрами в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
8. Появление сообщения "Обязательное поле" у поля "Телефон" при оставление поля пустым в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
9. Появление сообщения "Устаревший промокод" у поля "Промокод" при вводе устаревшего валидного промокода в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
10.Появление сообщения "Промокод не найден" у поля "Промокод" при вводе не валидного промокода в [форме записи](https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО" 
<a/>

**Сценарии тестирования API:**

1. Проверка статуса 200 и совпадения валидных* данных отправленных через UI [формы записи (https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО" с данными в body POST-запроса к серверу и новыми данными из БД. 
2. Проверка статуса 500 и отсутствие новых записей в БД при отправке пустого body в POST-запросе отправки [формы записи (https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
3. Проверка статуса 500 и отсутствие новых записей в БД при отправке пустого значения у атрибута phone в body в POST-запросе отправки [формы записи (https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
4. Проверка статуса 500 и отсутствие новых записей в БД при отправке пустого значения у атрибута name в body в POST-запросе отправки [формы записи (https://netology.ru/programs/qa#/order) на курс "Тестировщик ПО"
<a/>

**Примечание:*** Валидными значениями для полей являются:

- обязательное поле "Имя": латиница, кириллица, пробел и дефис/тире, заполненный минимум двумя буквами
- обязательное поле "Телефон": цифры, круглые скобки, пробел и дефис/тире в формате +9 (999) 999-99-99, от 9 до 14 символов включительно
- не обязательное поле "Промокод": латиница, кириллица, цифры и спецсимволы, кроме пробела
<a/>

## Перечень используемых инструментов с обоснованием выбора

 1. **IDE:** IntelliJ IDEA
 2. **Язык программирования:** Java
 3. **Система сборки:** Gradle (легче настраивать зависимости)
 4. **Тестовая среда:** TestNG (имеет, по сравнению с JUnit, больше аннотаций для управления состоянием SUT (например @BeforeSuite, @AfterSuite), может разбивать тесты на наборы тестов (suite) и имеет больше возможностей по параметризации тестов)
 5. **Система репортинга:** Allure (более сложные системы репортинга будут излишни)
 6. **Фреймворк для UI тестирования:** Selenide (популярный и простой инструмент)
 7. **Фреймворк для API тестирования:** REST Assured вместе с JSON Schema Validator (для отправки необходимых запросов и валидации JSON схемы)
 8. **Фреймворки для управления данными:** Java Faker (для генерации данных), необходимый драйвер (в зависимости от диалекта) для подключения к БД и DBUtils (для чтения записей с БД), Gson (для генерации body запросов при API тестирования)
<a/>

## Перечень необходимых разрешений/данных/доступов

 1. Разрешение на проведение автотестирования
 2. Доступ на чтения БД
 3. Доступ к существующим тестовым данным (если они есть)
<a/>

## Перечень и описание возможных рисков при автоматизации

 1. Появление "мусорных" записей в БД
 2. "Ложные" запросы к менеджерам на обратный звонок
 3. Дополнительная нагрузка на сервер 
 4. Потеря актуальности тестов при изменение UI сайта, особенно это касается переход к записи на курс через рекламный баннер
 <a/>

## Перечень необходимых специалистов для автоматизации

Данный проект не сложный, поэтому будет достаточно junior инженера по автоматизации, который знаком с основами необходимого инструментария, основами UI и API тестирования и базовыми навыками написания автотестов с использованием паттерна Page Object.

## Интервальная оценка с учётом рисков (в часах)

После согласования всех необходимых соглашений и доступов, у juniar специалиста написание тестов займет 16 - 24 часа.
