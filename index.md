## Welcome to my site

Here's a list of posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
	  
    </li>
  {% endfor %}
</ul>

<hr/>
<div class="blog list">
    <h1>Filed Under <small>#{{ page.tag }}</small></h1>

    {% for post in site.categories[page.tag] %}
        {% include post_preview.html %}
    {% endfor %}
</div>

<hr/>

<div>
{% for category in site.categories %}
  <div>
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article>
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>