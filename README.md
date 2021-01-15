# Deploy Keycloak to Heroku

This repository deploys the [Keycloak](https://www.keycloak.org) Identity and Access Manangement Solution 
to Heroku.  It is based of Keycloak's official docker image with some slight modifications to use the
Heroku variable for `PORT` and `DATABASE_URL` properly.

The deployment will be made with a free dyno (it won't run very well in smaller dynos
due to Java's memory hunger) 

This was originall forked from the [sannonaragao/keycloak-heroku](https://github.com/sannonaragao/keycloak-heroku) repo which used an attached Postgres database but this repo is updated to allow you to define the postgres data via jdbc connection string when deploying the project.

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

