![](https://telemetr.me/templates/svg/logo_full.svg)

## Примеры использования Telemetr API

**[Telemetr](https://telemetr.me)** - сервис глубокой аналитики
Телеграм-каналов.

### Доступ к API покупается отдельно

С 4 сентября 2026 года подписка на сайт доступа к API не даёт: API продаётся
отдельным пакетом. Пакет можно купить на любом тарифе, включая бесплатный, — витрина
с составом и ценами: [пакеты API](https://telemetr.me/premium-api?utm_source=user_api_docs&utm_medium=postman),
оформление — в [профиле](https://telemetr.me/profile/api/buy?utm_source=user_api_docs&utm_medium=postman).

Если пакета нет, любой метод отвечает **HTTP 429** и телом
`{"status": "error", "response": {"code": 0, "message": "Доступ к API не подключён…"}}`.
Это не превышение лимита и не временный сбой: повторы не помогут, нужен пакет. Тем, кто
оплатил подписку сайта до 4 сентября, лимиты сохранены до конца уже оплаченного периода.

Попробовать методы без покупки можно на нашем канале
[@telemetr_me](https://t.me/telemetr_me): пробный доступ отвечает по нему одному, с
небольшими лимитами, и даётся новым учётным записям на бесплатном тарифе. Формы ответов
в пробном режиме те же, что на платном пакете, — по ним видно, есть ли в наших данных
то, что вам нужно.

Сколько объёма осталось, всегда показывает `GET /v1/limits`, а после каждого вызова —
заголовки `X-RateLimit-*`.

Ссылки:

- [Регистрация в сервисе](https://telemetr.me/register?utm_source=user_api_docs&utm_medium=postman)

- [Документация к API](https://api.telemetr.me/doc?utm_source=user_api_docs&utm_medium=postman)

- [Инструкция Telemetr](https://help.telemetr.me/?utm_source=user_api_docs&utm_medium=postman)

- [Чат для пользователей API](https://t.me/telemetrAPI_chat)

- [Чат Telemetr](https://t.me/telemetr_chat)

- [Канал Telemetr](https://t.me/telemetr_me)
