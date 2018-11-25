# default_auth_laravel
# Setting up the environment
1. clone the git
2. composer update --no-scripts
3. cp .env.example .env
4. php artisan key:generate

# Note. 
use Illuminate\Support\Facades\Schema;
Then add the following schema inside the boot function

schema::defaultStringLength(191);
This will prevent from database error when migrated as the length will be 1024 and the mysql db gives default length 1000 
