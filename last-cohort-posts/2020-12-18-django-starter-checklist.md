---
layout: post
title: 🐴 Django Checklist 🐴 
tags: phase-2 python
---

## "Am I ready to start my Django app?" Checklist:
- [] Using the [Django Project Template](https://github.com/momentum-team-6/django-project-template-1)?
- [] Create an empty directory for the project
- [] `cd` into the empty directory
- [] Run `django-admin startproject --template=https://github.com/momentumlearn/django-project-template/archive/main.zip --name=Pipfile project .` replacing `project` with the name of the project
    - Creates the skeleton of your Django app in the directory, including an app directory called `core`, and a `templates` directory.
- [] Run `pipenv install`
    - Installs any requirements that are already on the `Pipfile`
- [] Run `pipenv shell`
    - Puts you inside the virtual environment, giving you access to all the requirements on the `Pipfile`.
    - You should see the name of the virtual environment inside `()` at the command prompt.
    - `pip freeze` can show you the python dependencies that you have access to inside that virtual environment.
- [] Run `cp project/.env.sample project/.env`
    - Makes the `.env` file to hold secret variable values by copying the sample file.
- [] Run `./manage.py makemigrations`
    - Creates instructions to build/change the database based on the models.
- [] Run `./manage.py migrate`
    - Applies migrations to the database.

Now, you're ready to start!

