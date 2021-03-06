---
title: USA Roadtrip App
subtitle: A simple app to explore America's cities.
date: "2018-12-18"
thumb_image: https://res.cloudinary.com/jacklyons123/image/upload/f_auto,q_auto/v1619951687/jacklyons.me/welcome-to-colorado.jpg
thumb_image_alt: An image of a "Welcome to Colorado" sign
image: images/successful-robin.png
image_alt: An image of the USA Roadtrip app
seo:
  title: Jack Lyons | USA Roadtrip App
  description: "In 2017 my wife and I spent six months living and road tripping across the United States. I decided to learn about\_Vue.js and build a USA Roadtrip App."
  extra:
    - name: "og:type"
      value: website
      keyName: property
    - name: "og:title"
      value: Jack Lyons | USA Roadtrip App
      keyName: property
    - name: "og:description"
      value: >-
        In 2017 my wife and I spent six months living and road tripping across
        the United States. I decided to learn about Vue.js and build a USA
        Roadtrip App.
      keyName: property
    - name: "og:image"
      value: /images/welcome-to-colorado.jpg
      keyName: property
      relativeUrl: true
    - name: "twitter:card"
      value: summary_large_image
    - name: "twitter:title"
      value: Jack Lyons | USA Roadtrip App
    - name: "twitter:description"
      value: >-
        In 2017 my wife and I spent six months living and road tripping across
        the United States. I decided to learn about Vue.js and build a USA
        Roadtrip App.
    - name: "twitter:image"
      value: /images/welcome-to-colorado.jpg
      relativeUrl: true
layout: project
---

[**Click here to view the project**](https://fluttering-farmer.glitch.me/)

_Note: this project is hosted for free on _[**_Glitch_**](http://glitch.com/)_, which means it might be asleep and therefore take just a little while to "wake up". Just hang in there til it loads._

In 2017 my wife and I spent six months living and road tripping across the United States. While we were on the road I decided to learn about the super-hot-and-trending [**Vue.js**](https://vuejs.org/) framework and build a USA Roadtrip App along the way. I gotta say, there’s a reason why Vue is so damn popular! It's a really great framework.

This project was built _without_ using [**Vuex**](https://vuex.vuejs.org/), the popular state management library. The reason _why_ I chose not to use it was because I wanted to find out first hand where and when the pain point/s exist as an application scales. Vuex is there to help manage state but sometimes it can be overkill for a simple application.  Once you've felt some of the pain points of passing state around in your app, you'll appreciate the need for Vuex. This app sat right on the Vuex cusp and I did start to notice some quirks when managing the "loading" state of the application. This was because data was being fetched by a parent component and then passed as props down to the child components but also emitted back up to the parent.

Another huge takeaway I gained from this experience was learning to handle asynchronous code. Fetching data from the Yelp API and passing it down into child components can get get messy quite fast. That's another side effect of an inefficiently management "state" - ala, without Vuex. Knowing which state should belong where (does it belong in a parent component or a child component?) is a tough question to answer. It is certainly worthwhile to take the time upfront to map out your application. _Some advice_: break down each component and try to understand what each does in the whole scheme of things.

If I had to choose a better code architecture, I would use Vuex upfront and create development and user stories for each component, plus I'd add Jest or Nightwatch into the mix to ensure the application runs as expected.

All in all, this was a really fun project and I would highly recommend you take a look at Vue.js!
