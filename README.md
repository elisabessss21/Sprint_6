# Sprint 6 — UI-автотесты Яндекс Самоката

Maven-проект автотестов учебного сервиса https://qa-scooter.education-services.ru/.

## Технологии

Java 11, Selenium WebDriver 4, JUnit 5, Maven, Page Object Model.

## Что проверяют тесты

- Раскрытие восьми вопросов FAQ и наличие ожидаемого текста в ответах.
- Оформление заказа через две кнопки «Заказать» с двумя наборами данных — четыре сценария.
- Появление сообщения «Заказ оформлен» после подтверждения.

## Структура

- `src/main/java/ru/praktikum/scooter/pages/` — `MainPage`, `OrderPage`, `RentPage`.
- `src/test/java/ru/praktikum/scooter/` — `BaseTest`, `FaqTest`, `OrderTest`.

## Запуск

Для запуска необходимы JDK 11, Maven и установленный браузер.

```bash
mvn test -Dtest=FaqTest -Dbrowser=chrome
mvn test -Dtest=OrderTest -Dbrowser=firefox
```

По умолчанию используется Chrome. Результаты предыдущих локальных проверок: восемь FAQ-сценариев прошли в Chrome; четыре сценария заказа — в Firefox.
