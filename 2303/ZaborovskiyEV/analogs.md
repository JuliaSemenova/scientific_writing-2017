## Сравнение существующих архитектур с точки зрения многопоточного программирования

### Монолитная архитектура
Тип архитектуры программная системы при котором она является единой и практически неделимой сущностью.

### Сервис-ореинтированная архитектура
Модульный подход к разработке программного обеспечения, основанный на использовании распределённых, слабо связанных заменяемых компонентов, оснащённых стандартизированными интерфейсами для взаимодействия по стандартизированным протоколам.

### Микросервисная архитектура
Архитектура в которой единое приложение представляется в виде набора небольших сервисов, каждый из которых работает в собственном процессе и коммуницирует с остальными используя легковесные механизмы.

## Критерии сравнения аналогов

### Согласованность
Данный критерий оценивался по тому, насколько просто в архитектуре поддерживать согласованность кода, обрабатывать ошибки и т. д. 

### Доступность 
Доступность подразумевает собой возможность функционирования системе при отказе части одной из её частей.

### Расширяемость 
Расширяемость подразумевает собой возможность добавлять новые или изменять уже готовые функции в системе

### Масштабируемость
Возможность размещения модулей системы на отдельных серверных узлах для увеличения производительности системы в целом.

### Параллелизм 
Параллелизм показывает наиболее привычный способ разнесения функционала по различным потокам. Стоит понимать, что данная характеристика не является абсолютным так, как ничто не мешает нам запустить все микросервисы в одном потоке.

## Таблица сравнения по критериям
Критерий\Архитектура | Монолитная | Сервис-ореинтированная | Микросервисная
------------ | ------------- | ------------- | ------------- 
Согласованность | Высокая | Средняя | Низкая
Доступность | Низкая | Средняя | Высокая 
Расширяемость | Низкая | Средняя | Высокая
Масштабируемость | Низкая | Высокая | Высокая
Параллелизм | Синхронизация средствами языка | Синхронизация средствами языка / Модуль-поток | Модуль-поток

## Выводы по итогам сравнения
В соответствии с приведенными выше данными каждое из решений имеет своими плюсы и свои минусы. Например, монолитная архитектура имеет высокую согласованность, а значит, гораздо проще в реализации, управлении и развёртывании. А микросервисная архитектура, хотя и не может быть легко развёрнута, но зато позволяет обновлять приложение по частям и даже если один из них сбоит, это не приводит к сбою всего приложения. Сервис-ореинтированная предоставляет собой некий баланс между вышеперечисленными так, как её модули более функциональны чем у микросервисной, но всё ещё не так сильно связаны, как у монолитной. Самые интересные характеристики это масштабируемость и параллелизм. Они показывают возможность разделения мощностей при сохраненнии логической целостности системы. Хотя микросервисная архитектура и будет иметь преимущества за счёт большой гибкости, но намного труднее из-за низкой связности. Обратное верно и для монолитной архитектуры. Поэтому, в процессе работы будет идти работа с сервис-ореинтированной архитектурой, как наиболее компромисным вариантом.

## Источники
1. paper_base/e-Reference.pdf
2. paper_base/akka-at-yandex.pdf
3. paper_base/microservices-for-java-developers.pdf
4. paper_base/Service Oriented Architecture with Java.pdf
5. paper_base/Evolve the Monolith to Microservices with Java and Node.pdf
