---
layout: dir
title: fiftysix.dev/friends
cmd: eza -laa
pwd: /friends
---
<!-- help me -->
{% assign current_folder = page.path | split: '/' | pop | join: '/' %}
{% assign badge_folder = current_folder | append: '/badges/' %}
{% assign badges = site.static_files | where_exp: "f", "f.path contains badge_folder" %}
{% assign sibling_pages = site.pages | where_exp: "p", "p.path contains current_folder" %}
<table class="term">
        <colgroup>
            <col class="col-perms">
            <col class="col-size">
            <col class="col-author">
            <col class="col-date">
            <col class="col-name">
        </colgroup>
        <tr>
            <td class="term ls-la">{% include dir.html %}</td>
            <td class="term ls-la size dash">-</td>
            <td class="term ls-la author">home</td>
            <td class="term ls-la date">{{ site.time | date: "%d %b %Y" }}</td>
            <td class="term ls-la"><a class="term-nav dir" href="">.</a></td>
        </tr>
        <tr>
            <td class="term ls-la">{% include dir.html %}</td>
            <td class="term ls-la size dash">-</td>
            <td class="term ls-la author">home</td>
            <td class="term ls-la date">{{ site.time | date: "%d %b %Y" }}</td>
            <td class="term ls-la"><a class="term-nav dir" href="/index.html">..</a></td>
        </tr>
        <tr>
            <td class="term ls-la">{% include dir.html %}</td>
            <td class="term ls-la size dash">-</td>
            <td class="term ls-la author">home</td>
            <td class="term ls-la date">{{ site.time | date: "%d %b %Y" }}</td>
            <td class="term ls-la"><a class="term-nav dir" href="#badges">badges</a></td>
        </tr>
    {% for item in site.data.friends %}
        <tr>
            <td class="term ls-la">{% include file.html %}</td>
            <td class="term ls-la size dash">-</td>
            <td class="term ls-la author">home</td>
            <td class="term ls-la date">{{ site.time | date: "%d %b %Y" }}</td>
            <td class="term ls-la"><a class="term-nav dir symlink" href="{{item.href}}">{{item.title}}</a></td>
        </tr>
    {% endfor %}
</table>

<div>
      {% include term-prompt.html pwd=page.pwd cmd="timg --grid 4x4 badges/*" id="badges" %}

      {% for item in site.data.badges %}
        <a class="badge" href="{{ item.url }}" aria-label="{{ item.name }}">
            <img src="/friends/badges/{{ item.badge }}" width=88 height=31 />
        </a>
      {% endfor %}
</div>

