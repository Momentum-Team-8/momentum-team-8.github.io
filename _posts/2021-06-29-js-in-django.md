---
layout: post
title: 🍔 Django with a Side of JavaScript 🍟
tags: phase-2 django javascript
---

## 🗓️ Today's topics

- Check in with progress on code snippets and flashcards
- Why and how to incorporate JavaScript into your Django application

## 🎯 Django Duplex Project

Habit Tracker or Code Snippets...continued.

## Resources

- [Django and AJAX](https://realpython.com/django-and-ajax-form-submissions/)
- [Fetching Data with Ajax and Django](https://www.brennantymrak.com/articles/fetching-data-with-ajax-and-django.html) -> This article is really helpful. There are really good code examples. Here are the most important bits:

  > By including the 'X-Requested-With' header set to 'XMLHttpRequest', the view will be able to check if the request is AJAX or not.

  ```py
    request.headers.get('x-requested-with') == 'XMLHttpRequest'
  ```
- [Django docs on the above](https://docs.djangoproject.com/en/3.2/ref/request-response/#django.http.HttpRequest.is_ajax)
- [Unintrusive JS with Django](https://lethain.com/intro-to-unintrusive-javascript-with-django/)

### ⭐ EXTRA/TMI

- [jQuery](https://jquery.com/) -> This is not something I _recommend_ using right now, but I include it here because a lot of the resources you will encounter about using JavaScript in a web browser will refer to it (like the article on unintrusive js listed immediately above). It is not as popular as it once was, and it is incompatible with a framework like React. But you will sometimes come across it, and you may end up working with it at your job, so you might as well recognize it when you see it and look it up if you ever need it.

## 🦉 Code

- [Example Django Music](https://github.com/Momentum-Team-8/example-django-music)
