## Welcome to Fishming's blog
This is my blog powered by 
I love using this web to show my recent researches.

<div id="page">
  <div id="body">
    {{ content }}
  </div>
</div>

<div id="related">
  <h2>Related Posts</h2>
  <ul class="posts">
    {% for post in site.related_posts limit:5 %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>