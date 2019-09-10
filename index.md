# Welcome to Fishming's blog
This is my blog powered by 
I love using this web to show my recent researches.

<html>
  <body>
    <div id='wrapper'>
      <div id='header'>
        <h2>Record the innovation</h2>
      </div>
      <div id='menu'>
        <ul>
          <li><a href='/'>Home</a></li>
          <li><a href='https://www.linkedin.com/in/仲明-于-4873b5187/' target='_blank' rel='me'>LinkedIn</a></li>
          <li><a href='https://me.csdn.net/weixin_43260254' target='_blank' rel='me'>CSDN</a></li>
          <li><a href='https://www.jianshu.com/u/1a1553cb9c70' target='_blank' rel='me'>JianShu</a></li>
        </ul>
      </div>
      <div id='content'>
        {{ content }}
        <div class='clearfix'></div>
      </div>
    </div>
    <div class="related">
      <h3>Related Posts</h3>
      <ul>
        {% for post in site.posts %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          <p>{{ post.excerpt }}</p>
        </li>
        {% endfor %}
      </ul>
    </div>
    <div id='footer'>
      Copyright &copy; 2019 fishming. Theme and code by <a href="http://github.com/fishmingyu">fishming</a>. Hosted by <a href='fishming.cn' target='_blank'>GitHub</a> and powered by <a href='http://github.com/mojombo/jekyll'>Jekyll</a>.
    </div>
  </body>
</html>