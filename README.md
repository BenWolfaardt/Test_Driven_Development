# Test Driven Development (TDD) with Python
Obey the testing goat: Using Django, Selenium and JavaScript by Harry J.W. Percival

> A book that I'm working my way through in the preperation for a new job where they make use of TDD. 

## Quick links
* [Book's site](https://www.obeythetestinggoat.com/)
* [Book by publisher](https://www.oreilly.com/library/view/test-driven-development-with/9781449365141/pr05.html)
* [Book's GitHub](https://github.com/hjwp/book-example/tree/master)

## Reminders

* `source venv/bin/activate` - activate venv environment
* `python manage.py runserver` - in a seperate terminal
* `python manage.py test` - run unit tests (UT)
  * `python manage.py test lists` - run unit tests (UT) after having moved the functional_tests into their own folder
* `python functional_tests.py` - run functional tests (FT)
  * `python manage.py test functional_tests` - run functional tests (FT) after having moved the functional_tests into their own folder

## Setup

> Please note that this project makes use of `venv` which is included in `.gitignore`

### Prerequisites

* [Firefox](https://www.mozilla.org/en-US/firefox/linux/?utm_medium=referral&utm_source=support.mozilla.org) - [guide](https://support.mozilla.org/en-US/kb/install-firefox-linux)
* [Geckodriver](https://github.com/mozilla/geckodriver) - [guide](https://askubuntu.com/questions/870530/how-to-install-geckodriver-in-ubuntu#871077)

### Venv

* `pip install "django<1.12" "selenium<4", "python-dotenv"`

### Django

* Project setup - `django-admin.py startproject superlists .`
* Start/create an app - `python manage.py startapp <app_name>`
* Create "migrations" (the thing that builds the database) - `python manage.py makemigrations`
* Create "migrations" for production (the thing that builds the database) - `python manage.py migrate`
