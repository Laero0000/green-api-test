# GREEN-API Test Page

Веб-страница для работы с методами [GREEN-API](https://green-api.com/) - сервиса для отправки сообщений через WhatsApp.

## Демо

**[https://bespoke-mermaid-b3fb38.netlify.app/](https://bespoke-mermaid-b3fb38.netlify.app/)**

## Функциональность

Страница реализует 4 метода GREEN-API:

| Метод | Описание |
|-------|----------|
| `getSettings` | Получить настройки инстанса |
| `getStateInstance` | Получить статус авторизации инстанса |
| `sendMessage` | Отправить текстовое сообщение в WhatsApp |
| `sendFileByUrl` | Отправить файл по URL в WhatsApp |

## Как использовать

1. Зарегистрируйтесь на [console.green-api.com](https://console.green-api.com/)
2. Создайте инстанс на тарифе **Developer** (бесплатно)
3. Отсканируйте QR-код через WhatsApp → привяжите номер
4. Откройте [страницу](https://bespoke-mermaid-b3fb38.netlify.app/)
5. Введите `idInstance` и `ApiTokenInstance` из консоли
6. Нажимайте кнопки - ответы API отображаются в поле справа

## Технологии

- Чистый HTML/CSS/JS - без фреймворков и зависимостей
- Прямые вызовы GREEN-API из браузера через `fetch`
- Нормализация номера телефона (принимает любой формат: `+7 (999) 123-45-67`)
- Обработка HTTP-ошибок с отображением статус-кода

## Документация GREEN-API

- [Метод getSettings](https://green-api.com/docs/api/account/GetSettings/)
- [Метод getStateInstance](https://green-api.com/docs/api/account/GetStateInstance/)
- [Метод sendMessage](https://green-api.com/docs/api/sending/SendMessage/)
- [Метод sendFileByUrl](https://green-api.com/docs/api/sending/SendFileByUrl/)
