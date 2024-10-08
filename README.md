
# Интернет-магазин

Этот проект представляет собой интернет-магазин, разработанный с использованием стека технологий: **React**, **Express**, **PostgreSQL** и **Node.js**. В проекте реализованы функциональные возможности как для клиентской, так и для серверной части, включая управление товарами, их отображение и взаимодействие с базой данных.

## Структура проекта

- **Frontend**: React.js
  - Компоненты для отображения каталога товаров, фильтрации, а также страницы управления товарами.
  - Bootstrap для стилизации и обеспечения адаптивности интерфейса.
  - MobX для управления состоянием приложения.

- **Backend**: Node.js, Express.js
  - RESTful API для взаимодействия с базой данных.
  - Маршруты для работы с пользователями, товарами, категориями и заказами.
  - Авторизация и регистрация пользователей.

- **Database**: PostgreSQL
  - Хранение данных о товарах, категориях, пользователях и заказах.
  - Использование Sequelize для ORM.

## Требования

- **Node.js** >= 14.x
- **npm** >= 6.x
- **PostgreSQL** >= 12.x

## Установка

1. Клонируйте репозиторий:

    ```bash
    git clone https://github.com/veganxjihad/web_shop_project.git
    ```

2. Перейдите в директорию проекта:

    ```bash
    cd 
    ```

3. Установите зависимости для серверной части:

    ```bash
    cd server
    npm install
    ```

4. Установите зависимости для клиентской части:

    ```bash
    cd client
    npm install
    ```

## Конфигурация

1. Настройте базу данных PostgreSQL:
   - Создайте новую базу данных.
   - Заполните данные для подключения в файле `.env` в папке `server`:

    ```plaintext
    DB_NAME=online_store
    DB_USER=postgres
    DB_PASSWORD=1
    DB_HOST=localhost
    DB_PORT=5432
    SECRET_KEY=random_secret_key123
    ```

2. Настройте переменные окружения для сервера:
   - Также в `.env` в папке `server` добавьте:

   ```plaintext
   PORT=4000
   SECRET_KEY=yrandom_secret_key123
   ```

## Запуск проекта

1. Запустите сервер:

    ```bash
    cd server
    npm run dev
    ```

    Сервер будет запущен на `http://localhost:4000` (в случае c MacOS порт 5000 может быть занят, можно запустить на 4000)

2. Запустите клиент:

    ```bash
    cd client
    npm start
    ```

    Клиентское приложение будет доступно на `http://localhost:3000`.

## Основные функции

- **Каталог товаров**: Просмотр и фильтрация товаров по категориям и брендам.
- **Корзина**: Добавление товаров в корзину и оформление заказа.
- **Админ панель**: Управление товарами и категориями (доступно только администратору).
- **Авторизация и регистрация**: Возможность создания аккаунта и входа в систему.

## Стек технологий

- **Frontend**: React, MobX, React Bootstrap
- **Backend**: Node.js, Express.js, Sequelize
- **Database**: PostgreSQL

