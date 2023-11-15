---
layout: page
title: PowerAppMaker.Dev
---

# Welcome to PowerAppMaker.dev

I decided to start this website aftering listening to an episode of a podcast called, **"A Question of Code"** in which the hosts were discussing top tips to enjoy what you do for new developers. I believe it was episode **87: Top Tips review: enjoy what you do** but don't hold me to that!

One of the tips that they discussed was the idea of new developer starting their own blog as a way to journal their successes and failures. The concept is that writing about a topic can help you wrap your head around it in a way that might not be possible otherwise. Some people write notes down on paper, others use apps like OneNote to write out helpful information that they can return to time and time again.

The advantage of using a blog as a way to improve your understanding of a topic has the added element of your words becoming public domain where other people can challenge you and tell you if you got it all wrong. It can be scary to put yourself out there, but it is great motivation to really try and understand the topic you are learning about. A blog is a great way to connect with other developers and build a precence for yourself.

This website... this blog is my attempt at documenting my learning journey for Microsoft Power Apps, SharePoint development and other related topics. I hope it will help me to build my knowledge of these products as I go from a beginner with some programming experience, mostly with web development, to an expert on these topics.

This is just the beginning... Much more to come! I hope PowerAppMaker.dev will help you on your own journey!
<br /><br />

## Recent Posts

<div>
  {% for post in site.posts %}
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
<br />
    </p>
  {% endfor %}
</div>

<a href="{{ "/articles/" | prepend: site.baseurl }}">View all Articles</a>
