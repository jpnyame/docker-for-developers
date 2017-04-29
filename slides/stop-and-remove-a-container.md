##  Stop and remove a container

* To stop a container:
<section>
<pre><code data-trim>
$ docker stop my-nginx
</code></pre>
</section>
* To restart an existing container:
<section>
<pre><code data-trim>
$ docker start my-nginx
</code></pre>
</section>
* To remove a container:
<section>
<pre><code data-trim>
$ docker rm my-nginx
</code></pre>
</section>
* Do not put data into the container. You use volumes to put data outside containers.

