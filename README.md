# PHP-Devcontainer-scaffold
Files for a VSCode devcontainer using PHP.

### NGINX
NGINX is used to host the php files. The `docker-compose.yml` file contains setup for the nginx service.
`nginx.conf` is setup in the `.devcontainer` folder and copied at build.
The `/public` folder at the root of the project is hosted by default. 

### PHP
PHP is setup as a service in `docker-compose.yml` and `PHP.Dockerfile`.
`Composer` is installed along with php mysql extensions.