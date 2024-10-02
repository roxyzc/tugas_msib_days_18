1. Clone Repository

    ```
    git clone https://github.com/roxyzc/tugas_days_18
    ```

2. Copy `.env.example` to `.env` and modify according to your environment
    ```
    cp .env.example .env
    ```
3. Settings your Database in .env
   | Kunci | value |
   |-------------------|---------------------|
   | `DB_HOST` | localhost |
   | `DB_PORT` | 3306 |
   | `DB_DATABASE` | Your Database Name |
   | `DB_USERNAME` | Your Username |  
   | `DB_PASSWORD` | Your Password |

4. Install composer dependencies
    ```
    composer install --prefer-dist
    ```
5. An application key can be generated with the command
    ```
    php artisan key:generate
    ```
6. Execute following commands to install other dependencies
    ```
    npm install
    ```
    ```
    npm run dev
    ```
7. Run these commands to create the tables within the defined database and populate seed data

    ```
    php artisan migrate --seed
    ```

8. php artisan serve --port=8080
