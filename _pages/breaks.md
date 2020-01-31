---
layout: default
id: breaks
title: Breaks
permalink: /breaks/
nav: true
nav-order: 2

intro: Here they are. A handpicked selection of Great British Breaks, perfect for that weekend away, from the northern wilds of Scotland down to the gorgeous beaches of Cornwall. Pick your break and don’t forget to make those memories last with your free trial of Touchnote.

sections:

  - id: iconic-british
    title: Iconic British
    description: From cockles at the seaside to a knees-up with locals in a Kentish country pub, there are some British holiday spots that are irresistibly timeless and wonderfully nostalgic. Dreamland whippy’s in Margate, wild walks in Lakeland, fish and chips in Whitby or catching a show in London’s West End, match your iconic British break with a stylish hotel.
    link: "#iconic-british-offers-on-se"

  - id: remote-wild
    title: Remote & Wild
    description: Fancy getting away from it all? Britain is home to some rather special secluded places, places where you feel like you’re the only one around for miles. From wild, Atlantic-battered islands in the Hebrides to the lesser-known landscapes of the Welsh Coastal Path, choose a break that really allows you to find a bit of peace and quiet. Pick from Manor houses, boutique cottages and more, all set in gorgeous surroundings for those long, back-to-nature days.
    link: "#remote-wild-offers-on-se"

  - id: spa
    title: Spa
    description: Sometimes nothing beats a few days in a spa. Letting yourself be pampered from head to toe, dipping into jacuzzis, pools, mud baths and saunas… If you can bear it, a spa getaway also comes with some other nice features. Beautiful hotels in lush surroundings, timeless spa towns filled with those other rejuvenating treatments – like shopping, fine dining and excellent bars; a spa getaway doesn’t need to just be sitting in a hot tub. Though, we wouldn’t blame you if that’s all you can manage...
    link: https://www.secretescapes.com/uk-spa-breaks/filter
---


<div class="container">
  <div class="vpad--xxl width width--xl text--center text--xxl">
    <p>{{page.intro}}</p>
    <p>Explain promo code lorem ipsum dolor sit amet consectetur adipisicing elit numquam.</p>
    <div class="promo-code">PROMOCODE</div>
    <a href="{{site.client.link}}" class="btn btn--cyan">Download the app</a>
  </div>
</div>

{% for item in page.sections %}
{% assign offers = site.data.offers[item.id] | sort: 'price' %}

<div class="{% cycle 'bg--light', '' %}">
  <div class="container vpad--xxl">
    <h2 class="title title--xl">{{item.title}}</h2>
    <p class="width--xl text--xxl">{{item.description}}</p>
    <div class="vpad--lg">
      <div class="row row--xl-6-6 row--gutters-lg">
        {% for offer in offers %}
          <div class="col">
            {% include offer/offer.html %}
          </div>
        {% endfor %}
      </div>
    </div>
    <div class="text--center">
      <a href="{{item.link}}" class="btn btn--orange">More {{item.title}} offers</a>
    </div>
  </div>
</div>

{% endfor %}