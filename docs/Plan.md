1. Перечень автоматизированых сценариев (сценарии 1.1 - 1.5 одинаковые для страницы Купить и Купить в кредит):
1.1 Проверка валидации формата а также наличия введеного номера.
1.2 Проверка валидации формата и корректроности ввода месяца а также наличия введеного значения. Формат должен быть 0 впереди если значение месяца одно знако место. Значение месяца может быть только в диапазоне 1..12. 
1.3 Проверка валидации формата и корректности введеного года а также наличия введеного значения. Формат должен быть двузначный а также з. Год не должен меньше текущего года и больше чем на 5 лет. 
1.4 Проверка наличия введеного имени пользователя
1.5 Проверка наличия введеного CVV кода а также формата (3 знака) и корректности (1..999).
2. Перечень используемых иструментов:
- IDE: IntelliJ IDEA 2023.2.4 (Community Edition)
- SDK: openjdk 11.0.21 2023-10-17
- Java проект с Gradle и следующими пакетами:
  - junit-jupiter:5.6.1 - основной фраймворк обеспечивает написание тестов 
  - selenide:6.17 - данный фраймворк позволяет запускать и манипулировать html элементами.
  - javafaker:0.15 - данный фраймровк позволяет генерировать случайные значения для вводимых полей (используеться для имени)
  - lombok:1.18.28 - данный фраймворк позволяет упростить написание дата классов без написания getter-в и setter-в 
  - mysql-connector-java:8.0.32 - пакет позволяет подключиться к MySQL бд 
  - postgresql:42.2.27  - пакет позволяет подключиться к Postgres бд
3. Перечень возможных рисков:
- не возможность тестирования проекта из за наличия критических ошибок не позволяющих написание тестов
- возможная несовместимость версий пакетов между собой а также орентированности на разные jdk
4. Интервальная оценка: 6 дня на UI тесты, 2 день на БД тесты, 8 дня на автоматизацию (Docker, Script)
5. План сдачи работ с выполнеными работами (4 недели):
   2 день. Созданы и настроен проект. Создан удаленного git репозиторий с всеми необходимыми файлами из задания
   10 день. Подготовлены скрипты для автоматизации: docker-compose.yml
   16 день. Выявлены зависимости (id, tag) на htmp странице для выборки необходимых элементов. Подготовлены основные PageObjeсt классы. А также разработаны UI тесты.
   20 день. Подключены не обходимые пакеты для подключения к БД. Также разработан класс для чтения настроек подключения к бд. Разработаты 4 db теста.
   27 день. Отладка и написание отчетов об найденных ошибок а также итоговая документация для сдачи
   28 день. Сдача проекта.     