Sept. 2020 - Backend Developer Technical Test
=============================================

The goal of this test is to assess your familiarity with building REST APIs and concepts related to building REST APIs with Django. You'll be building an API that enables any developer with an API Key to query the list of restaurants in a 3km radius given a set of GPS coordinates.

## Task
Your task is to build an API using the Django Rest Framework. Your API should contain the following endpoints:
* `/register/`: This endpoint receives `{name, username, password}` and creates an account from the information given.
* `/login/`: This endpoint receives `{username, password}` and responds with an access token that a client can use to authenticate themselves for subsequent calls.
* `/api_keys/` [login required]: A `GET` endpoint that responds with the current user's API Keys. Note that these keys (public and secret) are generated when a user creates an account.
* `/restaurants/` [API key pair required]: A `POST` endpoint that given `{lat, lng}` returns the list of restaurants in a 3km radius of those coordinates. Note that this endpoint is only accessible with a valid API key pair specified in the header with `X-Public-Key` and `X-Secret-Key` for the public and secret key respectively.

## Submission
To submit your work, send us a link to a git repository containing the code of your submission. The deadline for submissions is on **Tuesday 29th September 2020**.

Feel free to ask us any questions before or during the coding test, we'll be happy to help in any way we can.
