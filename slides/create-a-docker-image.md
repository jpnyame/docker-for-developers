##  Create a docker image

* In order to create your own docker image, you need to create a Dockerfile
* Build the image
<section>
<pre><code>
$ docker build -t zip-nginx:1.0
</code></pre>
</section>
* Create a new container based on the newly created image:
<section>
<pre><code>
$ docker run -d --name my-zip-nginx  -v /Users/jpnyame/Documents/docker/src:/usr/share/nginx/html:ro
-p 5000:80 zip-nginx:1.0
</code></pre>
</section>
