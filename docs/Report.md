Краткое описание: данное приложение позволяет провести тестирование web приложение по заказу и оплате туристуческой путевки.
Колличество тест-кейсов: 16 UI-тестов (успешных) и 2 теста с проверкой данных в базе данных для одного типа БД. 
Процент успешных и не успешных тест-кейсов: все успешные.
Общие рекомендации: нет.

Найден баг
Описание: сообщение об успешной операции не должно появляться после закрытия всплывающего окна об ошибке
Шаги для воспроизведения:
1) необходимо открыть страницу http://localhost:8080/
2) нажать на кнопку купить
3) Ввести данные карты с невалидным номером банковской карты
   ![image](https://github.com/n1ska/diploma/assets/130662674/53ad0b7b-594d-4cb0-b0ad-f737cc819142)
4) Нажать кнопку "Продолжить"
5) Появится всплывающее окно с ошибкой в правой верхней части страницы
   ![image](https://github.com/n1ska/diploma/assets/130662674/c18fe0dd-8c5e-420e-9357-e9e3ac5a77d9)
6) Нажать крестик на появивишемся окне с ошибкой, после закрытия данного окна появится сообщение об успешной операции
   ![image](https://github.com/n1ska/diploma/assets/130662674/59632e78-6bd2-43b7-a7f7-cf1a38ad2ed5)
 