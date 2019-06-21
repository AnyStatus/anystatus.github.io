<p class="lead">Recent Blog Posts</p>

{% for post in site.posts limit:5 %}
<p><a href="{{ post.url }}">{{ post.title }}</a></p>
{% endfor %}
