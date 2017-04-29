##  Start a new container

* Run your first container
<section>
<pre><code data-trim>
$ docker run -d --name my-nginx -p 5000:80 nginx:1.13.0-alpine 
$ docker ps -a 
</code></pre>
</section>
