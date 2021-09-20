<!DOCTYPE html>
<html>
  <head>
    <title>{% if page.title %}{{ page.title }} – {% endif %}{{ site.name }} – {{ site.description }}</title>

    {% include meta.html %}

    <!--[if lt IE 9]>
      <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:ital,wght@0,200;0,400;0,600;1,200;1,400;1,600&family=IBM+Plex+Sans:ital,wght@0,200;0,400;0,600;1,200;1,400;1,600&family=IBM+Plex+Serif:ital,wght@0,200;0,400;0,600;1,200;1,400;1,600&display=swap" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="{{ site.baseurl }}/basestyle.css" />
    <link rel="stylesheet" type="text/css" href="{{ site.baseurl }}/style.css" />
    <link rel="alternate" type="application/rss+xml" title="{{ site.name }} - {{ site.description }}" href="{{ site.baseurl }}/feed.xml" />

    <!-- Created with Jekyll Now - http://github.com/barryclark/jekyll-now -->
  </head>

  <body style="{% if page.bg-color %}--bg-color: #{{ page.bg-color }}; {% endif %}{% if page.fg-color %}--fg-color: #{{ page.fg-color }}; {% endif %}">
    <div class="wrapper-masthead">
      <div class="container">
        <header class="masthead clearfix">
          <!-- <a href="{{ site.baseurl }}/" class="site-avatar"><img src="{{ site.avatar }}" /></a> -->

          <div class="site-info">
            <h1 class="site-name"><a href="{{ site.baseurl }}/">{{ site.name }}</a></h1>
          </div>

          <nav>
            <a href="{{ site.baseurl }}/portfolio">Portfolio</a>
            <a href="{{ site.baseurl }}/blog">Blog</a>
            <a href="{{ site.baseurl }}/about">About</a>
          </nav>
        </header>
      </div>
    </div>

    <div id="main" role="main" class="container">
      {{ content }}
    </div>

    <div class="wrapper-footer">
      <div class="container">
        <footer class="footer">
          Thrasos Varnava 2021
          <a href="https://www.instagram.com/thrasv/">Instagram</a>
          <a href="https://www.behance.net/Thrasos">Bēhance</a>            
        </footer>
      </div>
    </div>

    {% include analytics.html %}
  </body>
</html>
