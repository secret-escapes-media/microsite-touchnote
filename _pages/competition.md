---
layout: competition
id: competition
title: Compet&shy;ition
permalink: /competition/
nav: true
nav-order: 4

long-title: Win a Great British Break
intro: Perched on a cliffside overlooking the beautiful Dorset coast, Gara Rock makes for a stylish getaway, with boutique appointments throughout. Spend three nights in the gorgeous Secret Suite, with a private terrace overlooking the sea and your very own hot tub for those sunset bubbles. It’s as private as you’d want, separate from the main hotel with its very own clifftop position for stunning views all round. To make things even more effortless, enjoy breakfast each morning and a two-course dinner with a bottle of wine on one night. Here’s your chance to reconnect with a loved one on this unmissable getaway. Enter now for your chance to win!
enter-cta: Enter Now

competition-form:
  id: comp
  post-url: "#getFormUrl"
  expiry-date: 2050-01-01
  fields:
    - id: name
      type: text
      label: Name
      required: true
    - id: email
      type: email
      label: Email
      required: true
    - id: qualify
      type: radio
      label: Are you a UK resident and over the age of 18?
      required: true
      options:
        - id: qualify-true
          label: 'Yes'
          value: 'yes'
        - id: qualify-false
          label: 'No'
          value: 'no'
          invalid: true
    - id: opt-in
      type: radio
      label: Would you like to receive emails from our Partner brand?
      required: true
      options:
        - id: opt-in-true
          label: 'Yes'
          value: 'yes'
        - id: opt-in-false
          label: 'No'
          value: 'no'
    - id: storytime
      type: text-long
      label: Tell us about your favourite travel experience
      required: true
    - id: eggs
      type: select
      label: What is your favourite continent?
      required: true
      options:
        - label: Africa
          value: africa
        - label: Antarctica
          value: antarctica
        - label: Asia
          value: asia
        - label: Europe
          value: europe
        - label: North America
          value: north-america
        - label: Oceania
          value: oceania
        - label: South America
          value: south-america
    - id: contact
      type: checkbox
      label: Do you have a preference on how we should contact you?
      required: true
      options:
        - id: contact-email
          label: Email
          value: email
        - id: contact-post
          label: Post
          value: post
        - id: contact-phone
          label: Phone
          value: phone
    - id: week
      type: select
      label: What is your favourite day of the week?
      options:
        - label: Monday
          value: mon
        - label: Tuesday
          value: tue
        - label: Wednesday
          value: wed
        - label: Thursday
          value: thur
        - label: Friday
          value: fri
        - label: Saturday
          value: sat
        - label: Sunday
          value: sun
  submit: Submit Entry
  terms: >
    By submitting your entry, you agree to the <a href="#" class="js-open-modal link--underlined" data-open-modal="competition-terms">terms and conditions</a> of this competition
---