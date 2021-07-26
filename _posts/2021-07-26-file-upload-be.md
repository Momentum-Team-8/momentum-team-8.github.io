---
layout: post
title: 🐝 Search, Uploads, & Automatic Deploys 🐝
tags: phase-3 phase-3-be full-text-search deploy file-upload
---

## Today's Topics

- Postgres full-text search
- Automatic deploys with Heroku's GitHub integration
- File upload and Amazon S3

## 🎯 Project: QuestionBox is due on Thursday

By today you should have working endpoints for:

- login and logout
- registration
- all questions
- all questions for a single user (authenticated user; own questions only)
- all answers for a single user (authenticated user; own answers only)
- create a question (authenticated users only)
- details for a single question
- all answers for a single question
- create an answer for a question (authenticated users only)

Depending on how you've constructed your API, you might have separate endpoints for all of the above, or you might have fewer endpoints (for instance, if you nested answers in the question detail endpoint). What matters is that your have endpoints your front-end team can use to access this data.

This week you should work on endpoints for:

- search all questions
  - optionally search questions and answers
- delete a question (for user who created the question)
- mark an answer as accepted (only if you are the author of the associated question)
- favorite/"star" a question (authenticated users only)

## 📖 Read | 📺 Watch | 🎧 Listen

- 📖 [File Upload with DRF](https://goodcode.io/articles/django-rest-framework-file-upload/)
- 🎧 + 📖 [Success with Static Files](https://www.mattlayman.com/django-riffs/success-static-files/)
- 📖 [Basic and Full-Text Search with Django and Postgres](https://testdriven.io/blog/django-search/)
  - 📖 [If you want A LOT more detail about full-text search in Postgres and Django, this blog piece has you covered](https://pganalyze.com/blog/full-text-search-django-postgres)
- 📖 [Blog post with more on full-text search](https://www.netlandish.com/blog/2020/06/22/full-text-search-django-postgresql/)
- [Search from the Ground Up](https://www.youtube.com/watch?v=is3R8d420D4&list=PL2NFhrDSOxgXXUMIGOs8lNe2B-f4pXOX-&index=2) -> DjangoCon 2019 video explaining search in detail
- 📖 [What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) -> Skim this -- this is Amazon's documentation and it gets really in-depth.
  - 📺 [Introduction to S3](https://www.youtube.com/watch?v=77lMCiiMilo) -> Also from Amazon

## 🔖 Resources

### `@action` decorator in ViewSets

- [DRF Docs: Marking extra actions for routing with the `@action` decorator](https://www.django-rest-framework.org/api-guide/viewsets/#marking-extra-actions-for-routing)
- [DRF Docs: Routing for extra actions](https://www.django-rest-framework.org/api-guide/routers/#routing-for-extra-actions)


### Filtering and search

- [DRF - Filtering](https://www.django-rest-framework.org/api-guide/filtering/) -> Pretty useful reference. Includes how to filter your output based on GET parameters, which you will want to do for using search terms.
- [Django Docs: full-text search & the search lookup](https://docs.djangoproject.com/en/3.2/ref/contrib/postgres/search/#the-search-lookup)
- [Django Docs: SearchVector](https://docs.djangoproject.com/en/3.2/ref/contrib/postgres/search/#searchvector) -> You'll need this if you want to search against more than a single field

### File uploads

- [Django Docs: ImageField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#imagefield)
- [Django Docs: FileField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#filefield)
- [Pillow: Python Imaging Library](https://pillow.readthedocs.io/en/stable/)
  - [`django-imagekit`](https://django-imagekit.readthedocs.io/en/latest/) -> If you want to resize images when they are uploaded, or do any kind of image processing, you will need this. Don't add it unless you know you need it.
- [How to Setup Amazon S3](https://simpleisbetterthancomplex.com/tutorial/2017/08/01/how-to-setup-amazon-s3-in-a-django-project.html)
- [`django-storages`](https://django-storages.readthedocs.io/en/latest/index.html)
- [DRF `FileUploadParser`](https://www.django-rest-framework.org/api-guide/parsers/#fileuploadparser)

#### POST with upload using Insomnia

- choose binary file attachment
- headers (this example assumes an image file in jpeg format, named `profile-photo  .jpg`):

  ```
  Content-Type: image/jpeg
  Content-Disposition: attachment; filename=profile-photo.jpg
  ```

For more information on the values for `Content-Type`:

- [MDN Content-Type Header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Type)
- [MDN MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)

#### CORS for file upload

Assuming you are using `django-cors-headers`, you'll need to add the following to `settings.py`:

```py

from corsheaders.defaults import default_headers

CORS_ALLOW_HEADERS = list(default_headers) + [
    'content-disposition',
]
```
