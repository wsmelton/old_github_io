## Welcome

You can use the [editor on GitHub](https://github.com/wsmelton/wsmelton.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

{% for post in site.posts %}
	<a href="{{ post.url }}">{{ post.title }}</a>
	{{ post.excerpt }}
{% endfor %}