---
layout: default
id: touchnote
title: TouchNote
permalink: /touchnote/
nav: true
nav-order: 3

banner:
  title: Send your Postcard
  title-sub: with TouchNote

intro: TouchNote allows you to instantly create custom-made postcards wherever you are in the world. What’s more, you can send those postcards instantly from the UK to your loved ones. So if you’re climbing a mountain in Kenya, or exploring a market in Delhi, capture the moment and share it with your loved ones.

features:

  - id: create
    title: Create
    description: Design the cards of your dreams, lovingly personalised with your photos and custom features, with designs created by TouchNote artists.

  - id: connect
    title: Connect
    description: Stay close to the ones you love by sending your creations far and wide, with free cards every month. No matter where you are in the world, postcards are sent from the UK for speedy delivery.

  - id: cherish
    title: Cherish
    description: TouchNote cards are printed to the highest quality, so you’ll have beautiful mementos to treasure for years. Nothing beats a physical greeting, a postcard hitting the doormat, with a personal message attached. Reconnect with your loved ones with TouchNote.

---

<div class="container">
  <div class="vpad--xxl width width--xl text--center text--xxl">
    <p>{{page.intro}}</p>
    <p>Explain promo code lorem ipsum dolor sit amet consectetur adipisicing elit numquam.</p>
    <div class="promo-code">PROMOCODE</div>
    <a href="{{site.client.link}}" class="btn btn--cyan">Download the app</a>
  </div>
</div>

<div class="bg--light">
  <div class="container vpad--xxl">
    {% for item in page.features %}
      <div class="bob{% cycle '', ' bob--swap' %}">
        <div class="bob__img">
          <div class="bg-img bg-img--4-3" style="background-image: url('{{site.img}}/img.jpg');">
            <a class="bg-img__link" href="{{site.client.link}}"></a>
          </div>
        </div>
        <div class="bob__text">
          <h2 class="title title--xl title--color">{{item.title}}</h2>
          <p class="text--xl">{{item.description}}</p>
          <div class="space--sm"></div>
          <a href="{{site.client.link}}" class="btn btn--sm btn--outline btn--outline-cyan">Find out more</a>
        </div>
      </div>
    {% endfor %}
  </div>
</div>