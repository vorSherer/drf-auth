# Lab 33 - Django REST Framework, Authentication and Production Server

### *Author: Thomas Sherer*, 2020-09-17

## Description - Overview
Let’s move our API closer to production grade by adding Authentication and switching to a Production Server

## Feature Tasks and Requirements
### Features - Django
- Add JWT Authentication to your API.
    - Install needed libraries in project configuration and/or site settings.

- Keep existing authentication so DRF Browsable API still usable.
    - That includes keeping the styling
    - Install needed libraries in project configuration and/or site settings.

### Features - Docker
- Create a boilerplate __`Dockerfile`__ and __`docker-compose.yml`__ so you don’t need to start from scratch each time.
- Switch to using [Gunicorn](https://gunicorn.org/) instead of Django’s built in development server.
    - mind the number of workers to avoid sluggishness

- __Warning__: You will run into styling issues when you switch over to Gunicorn.
    - On Django side you’ll need to properly handle static files.

- Adjust __`docker-compose.yml`__ so that data is persisted in a volume outside of container.

## Snippets
Refer to [SNIPPETS](https://codefellows.github.io/code-401-python-guide/curriculum/class-33/resources/SNIPPETS.html) as needed.

## Implementation Notes
### User Acceptance Tests
- Use tests from demo and adjust as needed for your project.
- Ensure tests pass

## Configuration
- Create new __`drf-auth`__ repository.
- Use __`poetry`__ to initialize __`drf-auth`__ project.
    - $ cd drf-auth

    - $ poetry init -n

- Use the folder __`drf-auth`__ as the root of your project’s git repository.

## Collaborations and Attributions

.gitignore content courtesy of https://www.toptal.com/developers/gitignore/api/django
