---
# Front Matter（必须用---包裹）
layout: home         # 使用home布局（通常由主题提供）
title: "我的博客"    # 首页标题
description: "记录技术与生活"  # 首页描述
permalink: /         # 首页路径（保持默认即可）
---

# 欢迎来到我的博客！ 👋

这里是首页的个性化内容，支持 **Markdown** 语法：

- [查看最新文章](/posts)
- [关于我](/about)

---

## 最新文章
<!-- 自动显示最近的5篇文章 -->
{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }})  
  <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}

