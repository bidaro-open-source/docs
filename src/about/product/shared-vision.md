# Общее видение

**Bidaro** - это английский открытый онлайн-аукцион, где пользователи могут делать ставки на лоты разных товаров. Здесь можно участвовать в торгах и выставлять свои товары, создавая активное сообщество покупателей и продавцов.

**Название Bidaro** объединяет `Bid` (ставка) и `aro` (лат. "собирать"), отражая суть платформы – объединение предложений и людей со всей Украины.

**Целевая аудитория Bidaro** состоит из украинцев в возрасте от 18 до 55 лет. Это пользователи со низким и средним уровнем дохода, которые хотят купить товар дешевле обычных магазинов или продать лишнее как можно дороже.

::: tip Почему английский аукцион?
Остальные виды аукционов не востребованы на украинском рынке. Аукцион с постоянным поднятием цены более понятен для целевой аудитории.
:::

## Ценность

Bidaro не создает особую ценность из-за специфики бизнеса, однако может выделиться среди конкурентов следующими способами:

- `Современный дизайн` - применение современного UI улучшит пользовательский опыт и привлечет новых пользователей.

- `Ставки в реальном времени` - новая ставка отобразится у всех пользователей, которые просматривают лот в реальном времени.

- `Быстрый и оптимизированный веб-сайт` - улучшит пользовательский опыт и повысит ранжирование в поисковой выдаче.

## Ответственность

Bidaro занимается только сведением покупателя и продавца, предоставив им платформу для торгов. Когда им нужно связаться между собой, они используют для этого телефон или почту.

## Монетизация

Bidaro взымает комиссию за сделку и это его единственный источник дохода.

Основные детали:

- Пользователи будут иметь свой личный балас на сайте.
- Начисление комиссии проходит в конце сделки с обоих сторон.
- Комиссия не может быть меньше 0.01 грн и больше 100 грн. В случаях выхода за пределы происходит округление.
- Если в течении месяца баланс будет отрицательным, аккаунт будет заморожен.

Расчет комиссии идет в процентах от итоговой стоимости товара:

| Итоговой стоимость лота | Комиссия
| -                       | -
| От 1 до 100 грн         | 3.5%
| От 100 до 1000 грн      | 3% + 1 грн
| От 1000 до 5000 грн     | 2.5% + 3 грн
| От 5000 и более         | 1.8% + 8 грн

## Функциональнось

Bidaro обладает следующими корневыми фукнциями:

- [Аутентификация](./authentication.md) - пользователи могут войти в свой аккаунт

- [Авторизация](./authorization.md) - пользователи имеют свои права, сгрупированные по ролям

- [Профили](./profiles.md) - пользователь может менять данные и следить за состоянием аккаунта через личный кабинет

- [Система лотов и торгов](./bidding.md) - пользователи могут выставлять свои лоты и учавствовать в торгах других

- [Каталог лотов](./catalog.md) - пользователи могут находить лоты через каталог сайта

- [Обслуживания](./maintenance.md) - пользователь имеет свой баланс и может оплатить услуги сайта

## Структура сайта

Основные:

- Главная страница (`/`) - описывает что такое Bidaro, его функции, как он работает и как им пользоваться.
- О нас (`/about`) - описывает создателей Bidaro, как он создавался и из чего состоит.
- Контакты (`/contacts`) - описывает контакты создателей Bidaro.
- Ответы на вопросы (`/faq`) - содержит ответы на популярные вопросы.
- Политика конфиденциальности (`/privacy-policy`)
- Правила пользования (`/terms-conditions`)

Бизнес:

- Каталог (`/catalog`) - содержит список лотов, способы их фильтрации и сортировки.
- Лот (`/lots/[lot-id]`) - содержит информацию про лот, сделанные ставки, время до конца торгов или информацию о победителе.

Внутренние:

- Личный кабинет (`/profile`) - содержит информацию о фио, аватар, статус верификации или блокировки, активные лоты и лоты с участием.
- Мои лоты (`/profile/lots`) - содержит список всех лотов пользователя, от активных до закрытых.
- Мои торги (`/profile/bidding`) - содержит список всех лотов, где пользователь принимал участие.
- Баланс (`/profile/balance`) - содержит информацию о списаниях и пополнениях баланса.
- Настройки (`/profile/setting`) - содержит формы для изменения данных пользователя.

Авторизационные:

- Вход (`/auth/signin`)
- Регистрация (`/auth/signup`)
- Восстановление (`/auth/reset`)
