# AWESOME MAXIMASTER

Если вам интересно получать уведомления о наших новых решениях, подпишитесь
в данном репозитории на релизы - будем делать их при добавлении сюда новых
репозиториев или существенных обновлениях в существующих.

## Обзор наших репозиториев

### Приложения

* [bitrix-cli-install](https://github.com/maximaster/bitrix-cli-install) -
  консольное приложение, которое позволит вам установить Битрикс прямо из
  консоли из дистрибутива или бекапа. Наличие запущенного веб-сервера не
  требуется;
* [twig.filewatcher](https://github.com/maximaster/twig.filewatcher) -
  консольное приложение, которое генерирует HTML-шаблоны из TWIG-файлов. Может
  быть настроена как Firewatcher в PHPStorm/Webstorm. Удобно, если нужно сразу
  делать простую вёрстку в TWIG с демо-данными;

### Профилирование и отладка

* [tideways-xhprof](https://github.com/maximaster/tideways-xhprof) - использует
  функции PHP расширения `tideways-xhprof`, чтобы сохранять информацию о времени
  выполнения кода для дальнейшего анализа производительности;

### Утилиты

* [atoa](https://github.com/maximaster/atoa) - универсальный конвертер любых
  данных в требуемый тип (примитив или объект);
* [func](https://github.com/maximaster/func) - коллекция полезных функций для
  работы со стандартными типами данных;
* [exceptior](https://github.com/maximaster/exceptior) - несколько функций
  упрощающих работу с исключениями в ряде сценариев;
* [alterator](https://github.com/maximaster/alterator) - упрощает поиск
  уникальных названий для объектов (например, при копировании объекта);

### Расширения сторонних решений

* [doctrine-migration-comparators](https://github.com/maximaster/doctrine-migration-comparators) -
  позволяет вручную сортировать выполнение миграций [doctrine/migrations](https://www.doctrine-project.org/projects/migrations.html)
  в разных пространствах имён, а так же относительно числовых значений версий;
* [jaft](https://github.com/maximaster/jaft) - универсальный
  [JSON:API](https://jsonapi.org) трансформер для
  [league/fractal](https://fractal.thephpleague.com/);
* [file-mailer-transport](https://github.com/maximaster/file-mailer-transport) -
  позволяет сохранять письма отправляемые через
  [symfony/mailer](https://symfony.com/doc/current/mailer.html) как EML-файлы
  для последующего просмотра (например через Thunderbird) и долгосрочного
  хранения;
* [cli-ent](https://github.com/maximaster/cli-ent) - Guzzle
  [handler](https://docs.guzzlephp.org/en/stable/handlers-and-middleware.html#handlers)
  позволяющий имитировать HTTP запросы в консольных приложениях;

### Битрикс

#### Автономные

* [tools.finder](https://github.com/maximaster/tools.finder) - функции для
  выборки из БД идентификаторов различных сущностей по символьным именам;
* [tools.events](https://github.com/maximaster/tools.events) - функционал для
  автоматической загрузки обработчиков событий Битрикс оформленных как
  статические методы класса с именем обрабатываемого события. См.
  [bitrix-event-dispatcher](https://github.com/maximaster/bitrix-event-dispatcher),
  если хочется оформлять более типизированные события и обособленные
  обработчики;
* [bitrix-sql-profile](https://github.com/maximaster/bitrix-sql-profile) -
  позволяет точечно профилировать конкретные хиты через Монитор
  производительности;
* [bitrix-enums](https://github.com/maximaster/bitrix-enums) - разные
  перечисления из ядра Битрикс, но при этом ядро не используется, что позволит
  использовать пакет в проектах без Битрикс, но которые с ним как-то
  взаимодействуют. Впрочем, помогает и в обычных Битрикс-проектах, чтобы не
  использовать
  [магические числа](https://en.wikipedia.org/wiki/Magic_number_(programming));
* [bitrix-loader](https://github.com/maximaster/bitrix-loader) - загружает
  Битрикс, получая информацию о DOCUMENT_ROOT из разных источников;
* [bitrix-cron](https://github.com/maximaster/bitrix-cron) - упрощает установку
  агентов на cron;
* [bitrix-ufo](https://github.com/maximaster/bitrix-ufo) - небольшая коллекция
  дополнительных UF-полей и интерфейсы для создания новых;
* [bitrix-reconnect](https://github.com/maximaster/bitrix-reconnect) - класс
  подключения к MySQL, который будет пытаться переподключиться настраиваемое
  количество раз при получении исключения `Bitrix\Main\DB\ConnectionException`;
* [bitrix-unstatic](https://github.com/maximaster/bitrix-unstatic) - извлечённые
  интерфейсы из существующих классов Битрикс, чтобы можно было подключать их как
  зависимости в ваших сервисах, при этом (а) загрузка ядра произойдёт лениво
  (б) нет никакой статики, как следствие на такой код легче написать unit-тесты;
* [bitrix-agent](https://github.com/maximaster/bitrix-agent) - типизированные
  интерфейсы работы с агентами (создание, чтение, обновление, удаление);
* [bitrix-orm-condition](https://github.com/maximaster/bitrix-orm-condition) -
  удобные классы для упрощения построения условий сложных ORM-запросов;
* [bitrix-table-classes](https://github.com/maximaster/bitrix-table-classes) -
  DataManager-классы для таблиц которые Битрикс пока не описал, описал плохо,
  либо заблокировал те или иные нужные методы;
* [bitrix-table-fields](https://github.com/maximaster/bitrix-table-fields) -
  дополнительные типы полей и валидаторы для ваших DataManager-таблиц;
* [bitrix-value-objects](https://github.com/maximaster/bitrix-value-objects) -
  [Value Object'ы](https://en.wikipedia.org/wiki/Value_object) для Битрикс, пока
  там только `ModuleId`;

#### Опирающиеся на другие крупные решения

* [tools.twig](https://github.com/maximaster/tools.twig) - позволяет
  использовать [Twig](https://twig.symfony.com) шаблоны в компонентах;
* [bitrix-migrations](https://github.com/maximaster/bitrix-migrations) -
  упрощает подключение на Битрикс-проект миграций через
  [doctrine/migrations](https://www.doctrine-project.org/projects/migrations.html)
  и содежит собственный базовый класс для миграций с рядом полезных методов под
  Битрикс;
* [bitrix-codeception](https://github.com/maximaster/bitrix-codeception) -
  модуль для [Codeception](https://codeception.com), который обернёт ваши тесты
  в транзакции;
* [bitrix-cli-commands](https://github.com/maximaster/bitrix-cli-commands) -
  консольные команды, которые можно подключить к `symfony/console`;
* [bitrix-event-dispatcher](https://github.com/maximaster/bitrix-event-dispatcher) -
  позволяет создавать и регистрировать события через
  [symfony/event-dispatcher](https://symfony.com/components/EventDispatcher).
  См. [tools.events](https://github.com/maximaster/tools.events), если требуется
  автономное решение;
  * [bitrix-events](https://github.com/maximaster/bitrix-events) - реализция для
    некоторых Битрикс событий для
    [bitrix-event-dispatcher](https://github.com/maximaster/bitrix-event-dispatcher);
* [bitrix-symfony-mailer](https://github.com/maximaster/bitrix-symfony-mailer) -
  позволяет использовать
  [symfony/mailer](https://symfony.com/doc/current/mailer.html) транспорты для
  отправки почты в Битрикс, например
  [file-mailer-transport](https://github.com/maximaster/file-mailer-transport);

### Временные решения

* [array-unique-shim](https://github.com/maximaster/array-unique-shim) -
  костыльно исправляет [баг](https://github.com/php/doc-en/issues/1463) из-за
  которого после `array_unique` вы можете получить массив с дубликатами;

### Устаревшее

* [tools.orm](https://github.com/maximaster/tools.orm) - позволяет делать
  выборку данных из инфоблоков вместе со свойствами. В новых версиях такое есть
  [из коробки](https://dev.1c-bitrix.ru/learning/course/index.php?COURSE_ID=43&LESSON_ID=12868&LESSON_PATH=3913.3516.5748.12864.12868);
* [bitrix-single-connect](https://github.com/maximaster/bitrix-single-connect) -
  в старых версиях Битрикс делает два подключения к MySQL (старое и новое `d7`).
  Данная библиотека обеспечивает наличие одного подключения;
* [tools.property_interfaces](https://github.com/maximaster/tools.property_interfaces) -
  набор интерфейсов, которые необходимо реализовать для разных вариантов
  исполнения пользовательских типов свойств. См.
  [bitrix-ufo](https://github.com/maximaster/bitrix-ufo);

## Общие подходы в наших репозиториях

* [PHP Coding Standards Fixer](https://cs.symfony.com) для проверки
  соблюдения кода стандартам форматирования;
* [Psalm](https://psalm.dev) для уточнения типов и их последующей проверки;
* [Devbox](https://www.jetify.com/devbox) для конфигурации воспроизводимого
  окружения;
* [Kahlan](https://kahlan.github.io/docs/) для написания unit-тестов;
* [семантическое версионирование](https://semver.org/);
