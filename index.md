## Welcome to my site

Here's a list of posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
	  
    </li>
  {% endfor %}
</ul>

