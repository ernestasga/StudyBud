FROM python:3.8-slim

LABEL Name=studybud
EXPOSE 8000

RUN apt-get update &&\
    apt-get install -y gettext libgettextpo-dev git build-essential autoconf libtool


WORKDIR /studybud

# Alias shoretning python manage.py command
RUN echo 'alias dj="python manage.py"' >> ~/.bashrc

RUN pip install pipenv

COPY Pipfile Pipfile.lock ./

RUN pipenv install --system --dev

COPY . /studybud
