# Базовый MVC-компонент Битрикс

Базовый компонент, предназначенный для простой реализации MVC. Основные функции:
* Обработка ЧПУ "из коробки" 
(при условии, что параметры компонента правильно настроены при подключении)
* Обработка входящих запросов в MVC-стиле с применением кеширования по-умолчанию
* Обработка и кеширование AJAX в коде компонента
* Обработка ошибок, перехват исключений
* Возможность наследования
* Легковесность, для начала работы достаточно знать API битрикс.

Компонент в первую очередь ориентирован на работу с ЧПУ, хотя его можно использовать 
и не для ЧПУ-функционала.

Компонент напрямую не используется. 
От него необходимо наследоваться, [создавая свой класс компонента](https://dev.1c-bitrix.ru/learning/course/?COURSE_ID=43&LESSON_ID=2028).

## Установка

``composer require digitalwand/mvc.base``, или просто скопируйте себе компонент в /bitrix/components/digitalwand/

## Основные понятия

Небольшая "таблица соответствий" между сущностями битрикса, элементами данного класса, и терминами MVC.
* Контроллер - класс компонента. Компонент в целом стоит считать контроллером. 
* Action (действие) - функция, которую выполняет контроллер, при переходе пользователя по определенному уру.
* Роутинг - определение какое действие какого контроллера должно быть запущено при переходе по урлу. 

## Документация и примеры

* [Простой пример использования](doc/ru/basic-usage.md)
* ["Продвинутое" использование](doc/ru/advanced-usage.md)
