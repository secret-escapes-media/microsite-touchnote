---
layout: default
id: overview
title: Overview
permalink: /
nav: true
nav-order: 1

banner:
  title: Great British Breaks
  title-sub: In partnership with TouchNote
---

<div class="container vpad--xxl">
  <div class="width width--xl text--center text--xxl">
    <p>{{site.description}}</p>
    <p>We’ve partnered with TouchNote not just to bring you the finest British breaks we can find, but to make that break all the more memorable. Whether you’ve climbed that Cumbrian peak and the view is too good not to share, or someone’s got ice cream all over their face at the seaside, turn the moment into a  custom postcard instantly. TouchNote will send it right away, connecting your special moments with the people you love.</p>
    <div class="space--sm"></div>
    <a href="{{site.baseurl}}/touchnote" class="btn btn--outline btn--outline-cyan">Find Out More</a>
  </div>
</div>

<div class="bg--light">
  <div class="container vpad--xxl">
    {% assign site-pages = site.html_pages | where: 'nav', 'true' | sort: 'nav-order' %}
    {% for item in site-pages %}
      {% unless page.id == item.id or item.id == 'competition' %}
        <div class="bob{% cycle '', ' bob--swap' %}">
          <div class="bob__img">
            <div class="bg-img bg-img--4-3" style="background-image: url('{{site.img}}/img.jpg');">
              <a class="bg-img__link" href="{{site.baseurl}}{{item.url}}"></a>
            </div>
          </div>
          <div class="bob__text">
            <h2 class="title title--lg">{{item.title}}</h2>
            <p class="text--xl">{{item.intro}}</p>
            <div class="space--sm"></div>
            <a href="{{site.baseurl}}{{item.url}}" class="btn btn--outline btn--outline-cyan">Find Out More</a>
          </div>
        </div>
      {% endunless %}
    {% endfor %}
  </div>
</div>