<div align="center">
  <h1> 
    Pinterest Clone
  </h1>
  <h3> 
    1536 × 864 / Vue 3 & FastAPI
  </h3>
</div>

<div align="center" style="margin-top: 10px;">
  <a href="https://pint3rest.xyz" target="_blank" rel="noopener noreferrer" style="margin: 0 15px; font-size: 1.2em; font-weight: bold; color: #8E44AD; text-decoration: none;">
      🌐 Pinterest 
  </a>
</div>

<div align="center">
  <a href="https://pint3rest.xyz/api/docs" target="_blank" rel="noopener noreferrer" style="margin: 0 15px; font-size: 1.2em; font-weight: bold; color: #8E44AD; text-decoration: none;">
    📚 API Docs
  </a>
  <a href="https://pint3rest.xyz/api/graphql" target="_blank" rel="noopener noreferrer" style="margin: 0 15px; font-size: 1.2em; font-weight: bold; color: #8E44AD; text-decoration: none;">
    🔥 GraphQL API
  </a>
  <a href="https://pint3rest.xyz/api/openapi.json" target="_blank" rel="noopener noreferrer" style="margin: 0 15px; font-size: 1.2em; font-weight: bold; color: #8E44AD; text-decoration: none;">
    📄 OpenAPI JSON
  </a>
  <a href="https://pint3rest.xyz/api/redoc" target="_blank" rel="noopener noreferrer" style="margin: 0 15px; font-size: 1.2em; font-weight: bold; color: #8E44AD; text-decoration: none;">
    📖 ReDoc
  </a>
</div>

![Логотип](.github/assets/overview.png)

## 📽 Обзор

🎬 **[Посмотреть демонстрационное видео на YouTube](https://youtu.be/3NwWrd8uvFQ)**


## 🛠️ Используемые технологии

### 🧩 Backend  
- **FastAPI** – REST и GraphQL API  
- **SQLAlchemy** – ORM для работы с базами данных  
- **Pydantic** – валидация данных и управление окружением  
- **JWT** – токены доступа/обновления с поддержкой отзыва  
- **OAuth2** – аутентификация через Google  
- **httpx** – взаимодействие с внешними API  
- **FastAPI-Cache** – кэширование на уровне API  
- **FastAPI-Mail** – отправка email через FastAPI  
- **GraphQL (Strawberry)** – GraphQL слой API  

### 🗄 Базы данных  
- **PostgreSQL**, **MySQL**, **MongoDB** – реляционные и нереляционные базы данных  
- **Redis** – кэширование, отзыв токенов, Celery брокер/результаты, RedBeat  

### ⏱ Асинхронные задачи и Realtime  
- **Celery** – асинхронные задачи: отправка email, обработка изображений  
- **Celery Beat** – периодические задачи (например, промо-емейлы)  
- **Redis Stream** – транспорт сообщений между Celery и FastAPI  
- **WebSockets** – чат в реальном времени с `FastAPI.websockets`  
- **SSE (Server-Sent Events)** – уведомления в реальном времени  
- **Asyncio**, **Aiofiles** – асинхронные операции  

### 🧪 Тестирование и качество кода  
- **Pytest** – тестовый фреймворк  
- **Ruff** – линтинг и форматирование  
- **Alembic** – миграции баз данных  

### 📦 Развертывание  
- **Docker**, **Docker Compose** – контейнеризация и оркестрация  
- **Nginx** – обратный прокси с маршрутизацией для API и WebSocket  
- **SSL** – безопасное HTTPS соединение  
- **VPS** – развертывание на виртуальном сервере  
- **GitLab CI/CD** – автоматизированный процесс сборки, линтинга, тестирования и развертывания  
- **Yandex S3** – хранение медиа-файлов (Yandex Object Storage)

### 🎨 Frontend  
- **Vue 3** – современный JavaScript фреймворк  
- **Pinia** – управление состоянием  
- **Vue Router** – маршрутизация  
- **Tailwind CSS** – утилитарный CSS фреймворк  
- **Axios** – HTTP клиент  

## 🌸 Лента
### Лента – основная страница с поиском и тегами, отображающая пины в виде GIF, видео и изображений. Она показывает пользователей, которые опубликовали эти пины. Макет выполнен в стиле masonry grid с бесконечной прокруткой.
<p align="center">
  <img src=".github/assets/feed.png" width="100%">
</p>

## 📌 Пин + Связанные  
### Детализированный пин с заголовком, описанием, ссылкой, тегами и пользователем, который его создал. Включает комментарии и лайки. Под пином отображаются связанные пины на основе общих тегов.
<p align="center">
  <img src=".github/assets/detail.png" width="100%">
</p>

## 🔍 Поиск
### Поиск пинов по запросу и тегам, с быстрым поиском, доступным на любой странице. Также отображаются популярные пины и список недавних поисков.
<p align="center">
  <img src=".github/assets/search.png" width="100%">
</p>

## ✨ Новый Пин
### Создание пина — изображение/GIF/видео, с возможностью добавления дополнительной информации и тегов.
<p align="center">
  <img src=".github/assets/create.png" width="100%">
</p>

## 👤 Профиль пользователя  
### Профиль пользователя — редактирование профиля владельцем, создание досок, просмотр/редактирование созданных/понравившихся/сохраненных пинов, просмотр/редактирование пинов на досках. Пользователи также могут подписываться/отписываться и писать сообщения другим пользователям.
<p align="center">
  <img src=".github/assets/user.png" width="100%">
</p>

## 👥 Подписчики/Подписки
### Просмотр подписчиков/подписок любого пользователя.
<p align="center">
  <img src=".github/assets/followers.png" width="100%">
</p>

## 🧷 Доски
### Пользователи создают доски и добавляют/удаляют пины на них
<p align="center">
  <img src=".github/assets/boards.png" width="100%">
</p>

## ⭐ Рекомендации
### Пользователи получают рекомендации в реальном времени на основе недавно просмотренных пинов.
<p align="center">
  <img src=".github/assets/recomendations.png" width="100%">
</p>

## 🔔 Обновления в реальном времени
### Пользователи получают обновления в реальном времени, когда их пины сохраняются, комментируются или лайкаются.
<p align="center">
  <img src=".github/assets/updates.png" width="100%">
</p>

## 💬 Чаты
### Создавая чат с другим пользователем, можно обмениваться сообщениями и медиа в реальном времени. Чаты можно настроить по размеру и цвету. Также можно увидеть, какие пользователи онлайн на сайте или в чате.
<p align="center">
  <img src=".github/assets/cahts.png" width="100%">
</p>

## 💬🔔 Обновления чатов
### На любой странице пользователь получает обновления о новых сообщениях от других пользователей.
<p align="center">
  <img src=".github/assets/chats_updates.png" width="100%">
</p>

## 📝❤️ Комментарии/Лайки
### Можно комментировать, лайкать и сохранять пины, а также комментировать и лайкать другие комментарии.
<p align="center">
  <img src=".github/assets/comments_likes.png" width="100%">
</p>

## Архитектура проекта
![Архитектура](.github/assets/architecture-pint3rest.jpg)

## Обсуждение  
Есть предложения или улучшения для проекта? Обсуждайте их в [разделе обсуждений](https://github.com/shutsuensha/pinterest-clone-vue3-fastapi/discussions)!

## Лицензия 
MIT License – свободно для использования и распространения!

## Контакты

Не стесняйтесь обращаться, если у вас есть вопросы, предложения или идеи для сотрудничества:

- Email: [dankupr21@gmail.com](mailto:dankupr21@gmail.com)
- Telegram: [@evalshine](https://t.me/evalshine)
- Linkedin: [daniil-kupryianchyk](https://www.linkedin.com/in/daniil-kupryianchyk-960594322)
