# Africa's Pocket Mid-Fullstack Engineer Code Challenge
## Pre-requisites
- Docker

## How to run
- Clone the repo
- Run `docker compose up` in the root directory
- In a new terminal session, run `docker compose exec app composer install`
- Copy `.env.example` to `.env` by running `docker compose exec app cp .env.example .env`
- Run `docker compose exec app php artisan key:generate`
- Run `docker compose exec app php artisan migrate`
- Run `docker compose exec app php artisan db:seed` to seed the database with dummy data. The command will create 100 users. Edit `\Database\Seeders\DatabaseSeeder` to change the number of users created.
- Navigate to `localhost:8000` in your browser to view the app
- PgAdmin is available at `localhost:5000` with the following credentials:
    - Email: `admin@gmail.com`
    - Password: `admin`
- Postgres is available at `pgsql:5432` with the following credentials:
    - Database: `laravel`
    - Username: `root`
    - Password: `password`
- Mailpit is available at `localhost:8025`
