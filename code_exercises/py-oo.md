---
title: Python Code Break 5
layout: default
---

## Define a User class and create user objects

Create a new python file and name it whatever you want. Write all the following code in that file.

For each step, before you move on to the next step, be sure you can create a new instance of your User class and see it printed to stdout or in the python shell.


### Step 1

Make a class named `User`. Add the following attributes to your class:

- `name`
- `email`
- `city`
- `state`

Create two different user instances using your class. How can you check their different attributes?

### Step 2

Add a `__str__` method to your class that displays the identity and attributes of an instance.

#### example

Say you have a `Game` class; the `__str__` method could look like this (although there are lots of other options!):

```python
def __str__(self):
    return f"<Game score={self.score} tries={self.tries}>"

```

### Step 3

Make a method named `location` that returns a string listing the user's city and state (e.g., "Durham, NC").

### Step 4

Add an attribute called `is_active` to your class. This attribute should have a default value of `True`.

Then, make another method called `deactivate` that changes the value of the `is_active` attribute to `False`.

Create an instance of a user and test that it works. Try resetting the attribute to `True` using the assignment operator and checking the value again.

### Step 5

Add an attribute called `login_count` that keeps a count of how many days in a row a user logs in. Its default value should be 0.

Add a method called `increment_login_count` that adds 1 to the `login_count` attribute each time it is called and returns the updated count.

Then add a method called `reset_login_count` that resets the count to 0.

Create an instance of a user and test that this works.
