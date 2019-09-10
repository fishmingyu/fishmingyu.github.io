# Welcome to Fishming's blog
This is my blog powered by 
I love using this web to show my recent researches.

<html>
  <head>
    <meta http-equiv="Content-type" content="text/html; charset=utf-8">
    <title>Scott Chacon - {{ page.title }}</title>
    <link rel="stylesheet" href="/stylesheets/master.css" type="text/css" media="screen" charset="utf-8"/>
    <script src="/javascripts/jquery.js" type="text/javascript" charset="utf-8"></script>
    <script src="/javascripts/jquery.github.js" type="text/javascript" charset="utf-8"></script>
    <link rel='alternate' type='application/rss+xml' href='http://feeds.feedburner.com/JoinTheConversation' />
  </head>
  <body>
    <div id='wrapper'>
      <div id='header'>
        <h1>Fishming</h1>
        <h2>Record the innovation</h2>
      </div>
      <div id='menu'>
        <ul>
          <li><a href='/'>Home</a></li>
          <li><a href='http://github.com/fishmingyu' target='_blank' rel='me'>GitHub</a></li>
          <li><a href='https://me.csdn.net/weixin_43260254' target='_blank' rel='me'>CSDN</a></li>
          <li><a href='https://www.jianshu.com/u/1a1553cb9c70' target='_blank' rel='me'>JianShu</a></li>
        </ul>
      </div>
      <div id='content'>
        {{ content }}
        <div class='clearfix'></div>
      </div>
    </div>
    <div id='footer'>
      Copyright &copy; 2019 fishming. Theme and code by <a href="http://github.com/mbleigh">fishming</a>. Hosted by <a href='fishming.cn' target='_blank'>GitHub</a> and powered by <a href='http://github.com/mojombo/jekyll'>Jekyll</a>.
    </div>
    <script type="text/javascript">
      var gaJsHost = (("https:" == document.location.protocol) ? "https://ssl." : "http://www.");
      document.write(unescape("%3Cscript src='" + gaJsHost + "google-analytics.com/ga.js' type='text/javascript'%3E%3C/script%3E"));
    </script>
    <script type="text/javascript">
      try {
        var pageTracker = _gat._getTracker("UA-82337-14");
        pageTracker._trackPageview();
        } catch(err) {}</script>
  </body>
</html>


<div class="related">
  <h3>Related Posts</h3>
  <table class="post-list">
    {% for post in site.related_posts limit:3 %}
      <tr>
        <th><a href='{{ post.url }}'>{{ post.title }}</a></th>
        <td>{{ post.date | date_to_string }}</td>
        <td><a href='{{post.url}}#disqus_thread'>Comments</a></td>
      </tr>
    {% endfor %}
  </table>
</div>