---
title: '🐍 Back-end: Deployment and PostgreSQL 🐍'
layout: post
tags: phase-3 phase-3-be deployment
category: back-end
---

## Topics

- deploying Django applications to [Heroku](https://www.heroku.com/)
- using [PostgreSQL](https://www.postgresql.org/)

## 🎯 Project: Habit Tracker

You'll be working on [Habit Tracker](https://classroom.github.com/a/mB8DZsoM) this week.

It's important to read the project requirements **thoroughly** and start to think about how you would do this project.

First steps: generate the project skeleton, get it deployed to Heroku, and design your models. Make sure to create a diagram showing model fields and relationships. _Talk through with each other_ how you are thinking about this.

By Thursday:

- Your application should be deployed to Heroku
- Your models should be done
- You should be able to create habits and associated daily records in the django shell (I recommend using `shell_plus`)

## 🔖 Resources

- [Example code: Django Recipes](https://github.com/momentum-team-7/example-django-recipes)
- [Checklist for deploying to Heroku](https://github.com/momentumlearn/student-resources/blob/main/articles/deploy-django-to-heroku.md)
- [`django-extensions` `shell_plus`](https://django-extensions.readthedocs.io/en/latest/shell_plus.html#shell-plus)
- [Momentum Django Project Template](https://github.com/momentumlearn/django-project-template)

### 📖 Read | 📺 Watch | 🎧 Listen

- [Full Stack Python: ORMs](https://www.fullstackpython.com/object-relational-mappers-orms.html)
- [Class-Responsibility-Collaborator Model (CRC)](http://agilemodeling.com/artifacts/crcModel.htm)
- [Entity Relationship Diagrams (ERD), from Lucid Chart](https://www.youtube.com/watch?v=QpdhBUYk7Kk)

### ⚡ Lightning Talk Topics

You should research these starting in the Django docs (linked below). For this talk, explain your topic and **show us a code example**. You may find a code example of each of these in the [Django Recipes](https://github.com/momentum-team-7/example-django-recipes) codebase.

Basic outline of your talk (you're welcome to vary this):

- Define your topic. What is it?
- How does this relate to other things you have learned before? (in other words, can you put it in context for everyone? How does this fit in?)
- Why do we care about this topic? When is it useful? Do you see it as being useful in this week's project or another project you've done in the past?
- How does it work?
  - Explain it conceptually.
  - **Show us some code**. The code example should demonstrate how to use it.
- Any thoughts you have about it that you want to share? Tell us what you think.

On Thursday, come prepared to talk for 5-7 minutes on your topic. If there are 2 people on your topic, come prepared to talk for 10-12 minutes.

- [Lookup expressions with `.filter()`](https://docs.djangoproject.com/en/3.1/topics/db/queries/#field-lookups) - Tori
- [Lookups that span relationships](https://docs.djangoproject.com/en/3.1/topics/db/queries/#lookups-that-span-relationships) - Tristan
- [Complex lookups with Q](https://docs.djangoproject.com/en/3.1/topics/db/queries/#complex-lookups-with-q-objects) - Dawud
- [Queries with Related objects](https://docs.djangoproject.com/en/3.1/topics/db/queries/#related-objects) - Mike
- [Aggregate & Annotate](https://docs.djangoproject.com/en/3.1/topics/db/aggregation/) - Ben and Grant
