---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---


### Die letzten Posts
{% for post in site.posts %}
 [{{ post.title }} ({{ post.date | date: "%-d.%-m.%Y" }})]({{ post.url | prepend: site.baseurl }})
 
 {{ post.summary }}
{% endfor %}
