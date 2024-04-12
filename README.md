## 🛠️ Установка

### Предварительные требования

* [PHP ^8.1](https://www.php.net/manual/ru/install.php)
* [Composer (v2+)](https://getcomposer.org/doc/00-intro.md)
* [Node.js (v16+)](https://nodejs.org/en) & [NPM (9+)](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
* SQLite for local, MySQL or PostgreSQL for production

### Локальная установка

1. Склонируйте репозиторий проекта
```sh
git clone https://github.com/gitkulikov/auction.git
```

2. Перейдите в директорию проекта
```sh
cd auction
```

3. Скопируйте файл .env.example и переименуйте его в .env
```sh
cp .env.example .env
```

4. Укажите параметры подключения к БД в файле .env
```sh
DB_CONNECTION=sqlite
```

5. Установите зависимости, используя Composer
```sh
composer install
```

6. Установите зависимости, используя Npm
```sh
npm install
```

7. Запустите сборку фронтенд-ресурсов в режиме разработки
```sh
npm run dev
```

8. Сгенерируйте ключ приложения
```sh
php artisan key:generate
```

9. Примените миграции и заполнените данные сидерами
```sh
php artisan migrate --seed
```

10. Запустите локальный сервер разработки
```sh
php artisan serve --port=8822
```

-----

## 🖥️ Руководство пользователя

Для удобства тестирования и ознакомления с приложением, вы можете использовать следующие учетные данные для входа в систему:

* Логин: admin@admin.com
* Пароль: password

-----

## 🖥️ Руководство разработчика

Для добавления или обновления русской локализации, необходимо выполнить команду:
```sh
php artisan lang:add ru
```