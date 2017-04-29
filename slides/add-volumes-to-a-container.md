##  Add volumes to a container

* You can attach local volumes to your container and persist your data:
<section>
<pre><code data-trim>
$ docker run -d --name my-nginx -v /Users/jpnyame/Documents/docker/nginx.conf:/etc/nginx/nginx.conf:ro -v /Users/jpnyame/Documents/docker/src:/usr/share/nginx/html:ro -p 5000:80 nginx:1.13.0-alpine
</code></pre>
</section>
