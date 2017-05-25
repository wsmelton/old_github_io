## Welcome

This is a basic blog that has no fancy bells and whistles. 

{% for post in site.posts %}

	<a href="{{ post.url | prepend: site.baseurl }}
	<h2>{{ post.title }}</h2>
	{{ post.excerpt }}
	<p>
	Posted on {{ post.date | date_to_string }}
	</p>
{% endfor %}
