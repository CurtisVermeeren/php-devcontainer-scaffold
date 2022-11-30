# PHP-Devcontainer-scaffold
Files for a VSCode devcontainer using PHP.

### NGINX
NGINX is used to host the php files. The `docker-compose.yml` file contains setup for the nginx service.
`nginx.conf` is setup in the `.devcontainer` folder and copied at build.
The `/public` folder at the root of the project is hosted by default. 

### PHP
PHP is setup as a service in `docker-compose.yml` and `PHP.Dockerfile`.

`Composer` is installed along with php mysql extensions.

`xdegu` is installed in the `PHP.Dockerfile`.

### MYSQL
MariaDB is used in place of MySQL. Edit the `database.env.TEMPLATE` file with the database information and rename to `database.env`.

Port `3306` is exposed to connect with a client such as MySQL Workbench.

### Laravel 

Create new Laravel projects using the command `composer create-project --prefer-dist laravel/laravel my-project` and replacing your project name.