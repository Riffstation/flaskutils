# Flask-Philo

Small and very opinionated framework to build flask based microservices.

## What this project is about?

Flask is an awsome web microframework that works great out of the box. Nevertheless,
additional configuration and integration with complementaries libraries are required 
in order to build complex applications. Here in [riffstation.com](play.riffstation.com) we have several
HTTP REST based microservices, anytime that we want to create a new microservice we need to bootstrap
very similar common code.

This framework collect all the logic related with HTTP, REST and data access in one common place.
Feel free to use it and extendent it. We are willing to hear about your suggestions and improvements.

## Executing test

In order to run test a vagrant instance is required, below steps required to execute unit tests:

```
   cd test
   vagrant up
   vagrant ssh
   cd /src/test
   python3 manage.py test
```


## Basic Features

* REST out of the box.

* Simple sqlalchemy orm customized for postgresql with multiple dabatases.

* Simple Redis integration.

* Simple Elastic Search integration.

* Basic AWS integration.


## External Resources

* [Flask Website](http://flask.pocoo.org/)

* [Flask Book](http://flaskbook.com/)

* [SQL Alchemy](http://www.sqlalchemy.org/)

* [Python Redis](https://pypi.python.org/pypi/redis/2.10.3)

* [Python Elastic Search](https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/index.html)

* [AWS Boto](https://pypi.python.org/pypi/boto3)


## Creating a new project
Flaskutils includes the `flaskutils-admin` command line tool.
To quickly generate a new flaskutils project, navigate to the directory in which you want to create the project and run:

```
flaskutils-admin startproject <project_name>
```

This will create a folder called project_name which will contain the basic structure of a flaskutils application, including a Vagrantfile, basic unit tests and bdd tests and configuration.
