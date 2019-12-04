---
layout: Blog
title: Blog Page.
permalink: Blog.html
description: "Alltechnotricks is the best place on the internet where you learn all the tips & tricks right from starting a blog to making money online legitimately for free of cost."
image: upload/karunakar-patel-blog-image.png
datepublished: "2019-11-25"
datemodified: "2019-11-25"
---
{% for post in site.posts %}

<article
      class="post-card post tag-challenge tag-code tag-code-challenge tag-coding tag-css tag-html tag-interview tag-coding-interview tag-interviewing tag-javascript tag-job tag-job-hunting tag-job-interview tag-learning-to-code tag-learn-to-code ">
      <a class="post-card-image-link" href="{{post.url | absolute_url}}">
       <img class="post-card-image" srcset="{{post.image}}" sizes="(max-width: 1000px) 400px, 700px"
        onerror="this.style.display='none'" alt="{{post.title}}" title="{{post.title}}" />
      </a>
      <div class="post-card-content">
       <div class="post-card-content-link">
        <header class="post-card-header">
         <h2 class="post-card-title">
          <a href="{{post.url | absolute_url}}">
           {{post.title}}
          </a>
         </h2>
         <span class="post-card-tags">
         <p>{{post.description | truncate: 100 }}</p>
         </span>
        </header>
       </div>
<footer class="post-card-meta">
        <ul class="author-list">
         <li class="author-list-item">
          <div class="author-name-tooltip">
           Karunakar Patel.
          </div>
          <a href="https://www.alltechnotricks.com" class="static-avatar">
           <img class="author-profile-image" src="uploads/avatar.png" alt="Karunakar Patel" />
          </a>
         </li>
        </ul>
        <a class="meta-item" href="https://www.alltechnotricks.com">Karunakar Patel</a>
        <time class="meta-item">Last Update: {{post.datemodified | date_to_string}}</time>
      </footer>
	      </div>
     </article>

{% endfor %}
