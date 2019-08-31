---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<ul class="post-list">
    {% for post in site.posts %}
      <div class='post'>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <span class="post-meta">
          {{ post.date | date: "%b %-d, %Y" }} {{ post.author }}
        </span>
        <br>
        <img src="{{ site.baseurl }}{{ post.image }}">
        <br>
        <span>
          {{ post.excerpt }} <a href="{{ post.url | prepend: site.baseurl }}">Keep reading</a>
        </span>
      </div>
    {% endfor %}
    
  </ul>
