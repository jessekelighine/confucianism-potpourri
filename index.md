---
title: "《論語雜論》"
author: "<a href=\"https://jessekelighine.com\"><code>jessekelighine.com</code></a>"
layout: default
---

<nav id="TOC" role="doc-toc">
  <ul>
    <li><a href="#prologue">序</a></li>
    {% for post in site.posts reversed %}
    {% assign anchor = post.anchor | default: post.date | date: "%Y-%m-%d" %}
    <li><a href="#{{ anchor }}">{{ post.title }}</a></li>
    {% endfor %}
    <li><a href="#comments">留言板</a></li>
  </ul>
</nav>

# 序 {#prologue}

因為太常有事沒有就在想一些《論語》或是《四書》的內容，
便有了稍微有系統地把這些雜念寫下來的念頭。
這些討論大概都不是我原創的，
而且很多應該都是從[傅佩榮教授](https://zh.wikipedia.org/zh-tw/%E5%82%85%E4%BD%A9%E6%A6%AE)的書或是講座中得到的啟發。
其餘的部分可能對很多人來說都顯而易見，
只是因為我以前沒有認真思索過，
所以突然開竅了才覺得頗有感觸。
當然我也不是什麼專家學者，這些觀點也不見得有多正確，
只是因為我記性不好，所以還是決定把它們寫下來以便日後參考。

<!-- POSTS START HERE  -->

{% for post in site.posts reversed %}
{% assign anchor = post.anchor | default: post.date | date: "%Y-%m-%d" %}
<h1 id="{{ anchor }}">{{ post.title }}</h1>
{{ post.content }}
{% endfor %}

# 留言板 {#comments}

<script src="https://giscus.app/client.js"
        data-repo="jessekelighine/jessekelighine.github.io"
        data-repo-id="R_kgDOLmNjDQ"
        data-category="General"
        data-category-id="DIC_kwDOLmNjDc4CmBxT"
        data-mapping="pathname"
        data-strict="1"
        data-reactions-enabled="0"
        data-emit-metadata="0"
        data-input-position="bottom"
        data-theme="light"
        data-lang="zh-TW"
        crossorigin="anonymous"
        async>
</script>
