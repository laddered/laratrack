# LaraTrack 🛠️

**LaraTrack** — это pet-проект на Laravel, предназначенный для строгого контроля и отслеживания задач. Проект построен на Laravel 11, Docker и предоставляет REST API для управления пользователями, задачами, ролями и статусами.

---

## 📌 Основные особенности

- 🧱 Laravel 11 + Docker
- 🔐 Аутентификация через Laravel Sanctum (SPA-ready)
- ⚙️ Очереди на Redis + Horizon
- 📦 PostgreSQL / Redis / Mailhog в Docker
- 📑 Swagger-документация API
- 🧪 Тестирование с Pest
- 🧑‍⚖️ Ролевой доступ (admin, manager, performer)
- 🧾 Журнал активности (activity log)
- 🌐 Отдельный фронтенд на Vue 3 (SPA)

---

## 🐳 Стек и технологии

| Слой       | Технологии |
|------------|------------|
| Backend    | Laravel 11, Sanctum, Horizon, Telescope |
| Frontend   | Vue 3, Vite, Pinia, Vue Router |
| Database   | PostgreSQL |
| Queue/Cache| Redis |
| Dev Tools  | Mailhog, Swagger, Docker Compose |
| Тесты      | PestPHP |
| Документация | L5 Swagger |

---

## 🚀 Быстрый старт

### 🔧 Требования

- Docker + Docker Compose
- Make (опционально)

### ⏱ Установка

```bash
git clone https://github.com/your-username/laratrack.git
cd laratrack
cp .env.example .env
./vendor/bin/sail up -d
php artisan key:generate
