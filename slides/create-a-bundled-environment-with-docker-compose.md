##  Create a bundled environment with docker-compose

* You can create a development environment with multiple images in one single step
* Docker-compose allows you to describe images features and dependencies in a docker-compose.yml file.
<section>
<pre><code>
version: "2"
services:
  my-wpdb:
    image: mariadb
    ports:
      - "3306:3306"
    environment:
      MYSQL_ROOT_PASSWORD:root
  my-wp:
  depends_on:
    - my-wpdb
    image: wordpress
    volumes:
      - ./:/var/www/html
    ports:
      - "8080:80"
    links:
      - my-wpdb:mysql
    environment:
      WORDPRESS_DB_PASSWORD:root
</code></pre>
</section> 
* Type the command:
<section>
<pre><code data-trim>
$ docker-compose up -d
</code></pre>
</section>
