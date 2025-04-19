# Yadino Backend

> Laravel 12 RESTful API for the open-source Yadino mobile to-do app.

This is the backend service powering [Yadino](https://github.com/RahimMahmoudzadeh/Yadino), a to-do list mobile app. It provides APIs for user authentication, task management, and data synchronization with the mobile client.

---

## 🔧 Tech Stack

- **Framework:** Laravel 12
- **Language:** PHP 8.2+
- **Database:** MySQL (or MariaDB)
- **Authentication:** Custom JWT implementation with Firebase JWT for decoding and validation, and support for Google Sign-In
- **Queue/Cache:** Redis
- **Testing:** PHPUnit, Laravel Test Utilities

---

## 📋 Requirements

- PHP >= 8.2
- Composer
- MySQL / MariaDB
- Laravel CLI
- Redis

---

## 🚀 Installation

```bash
git clone https://github.com/alimousavidev/Yadino.git
cd Yadino-backend
cp .env.example .env
composer install
php artisan key:generate
```

Update your `.env` file with your database and other environment settings.

---

## ▶️ Running the App

```bash
php artisan migrate
php artisan serve
```

The API will be available at: `http://localhost:8000`

---

## 📚 API Documentation

API documentation will be added soon.

---

## 🧪 Running Tests

```bash
php artisan test
```

or

```bash
vendor/bin/phpunit
```

---

## 📂 Project Structure

```
app/
├── Http/
│   ├── Controllers/
│   └── Middleware/
├── Models/
routes/
├── api.php
```

---

## 🛠 Deployment

To deploy this project in a production environment:

1. Set appropriate `.env` values
2. Run `composer install --optimize-autoloader --no-dev`
3. Run `php artisan migrate --force`
4. Set permissions for `storage/` and `bootstrap/cache/`
5. Use a process manager for queue workers if needed
6. Serve with a web server like Nginx or Apache

---

## 🤝 Contributing

We welcome contributions from the community!

### Branch Naming Convention

- `feature/<feature-name>` – New features
- `fix/<bug-description>` – Bug fixes
- `chore/<task>` – Maintenance tasks
- `hotfix/<urgent-fix>` – Critical patches

### Commit Message Format

Use [Conventional Commits](https://www.conventionalcommits.org):

Examples:
- `feat(auth): implement token-based login`
- `fix(task): correct due date handling`
- `chore(env): update .env.example`

### How to Contribute

1. Fork this repository
2. Create a new branch: `feature/<your-feature>`
3. Commit your changes
4. Push to your fork
5. Submit a Pull Request

---

## 📄 License

This project is licensed under the [GNU General Public License v3.0](LICENSE).

---

## 👥 Maintainers

- [@Rahim Mahmoudzadeh](https://github.com/RahimMahmoudzadeh) – Mobile Frontend Developer
- [@Ali Mousavi](https://github.com/alimousavidev) – Backend Developer
