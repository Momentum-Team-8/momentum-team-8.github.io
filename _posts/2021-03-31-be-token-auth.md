---
layout: post
title: 🐍 Authentication & Authorization 🐍
tags: phase-3 phase-3-be
---

## Today's Topics

- Setting permissions classes in views in DRF
- Token authentication in DRF with djoser
- CORS headers
- Full-text search

## 🎯 Project

Keep on with QuestionBox! You should be able to return questions and answers at least by tomorrow.

## 📖 Read | 📺 Watch | 🎧 Listen

- [Finally Understand auth in DRF - a Will Vincent talk](https://www.youtube.com/watch?v=pY-oje5b5Qk) -> Will isn't using the djoser library but he does a great job of reviewing different auth strategies and why you would choose one or the other. Watch this for a better understanding and overview of auth.

## 🔖 Resources

#### Permissions

- [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)
- [Pro-Tip: Logical operators with DRF Permissions](https://www.revsys.com/tidbits/tip-about-drf-permissions/)

#### Authentication

- [Djoser documentation](https://djoser.readthedocs.io/en/latest/)
- [DRF docs: Token-based authentication](https://www.django-rest-framework.org/api-guide/authentication/#tokenauthentication)
- [The Ultimate Tutorial for Django REST Framework: Login and Authentication](https://sunscrapers.com/blog/django-rest-framework-login-and-authentication/)

#### CORS

- [MDN CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
  - [MDN Access-Control-Allow-Origin Header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Origin)
  - [Julia Evans comic explaining CORS better than MDN does](https://twitter.com/b0rk/status/1162392625057583104?lang=en)

#### Filtering and search

- [DRF - Filtering](https://www.django-rest-framework.org/api-guide/filtering/) -> Pretty useful reference. Includes how to filter your output based on GET parameters, which you will want to do for using search terms.
- [Django docs: full-text search & the search lookup](https://docs.djangoproject.com/en/3.1/ref/contrib/postgres/search/#the-search-lookup)
- [Blog post with more on full-text search](https://www.netlandish.com/blog/2020/06/22/full-text-search-django-postgresql/)
  - [If you want A LOT more detail about full-text search in Postgres and Django, this blog piece has you covered](https://pganalyze.com/blog/full-text-search-django-postgres)
