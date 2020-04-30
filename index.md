## Welcome to My GitHub Page - agoiz.tech



Thanks for visiting.
Basically this is a very simple page to host a blog regarding IT Technical stuff.
Some of the content might be related to my present or past projects.
Other content will be related to my own investigation and interests.
Hope you enjoy and let me know if you would like me to cover any topic.

***
### Links to my posts below:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

***
Built thanks to Github pages.
