pyzip-demo-apb
======================

An apb for deploying a simple [Python Zip App Demo](https://hub.docker.com/r/ansibleplaybookbundle/pyzip-demo/) app that can bind to Postgres for testing purposes.

## What it does
* Deploys a bindable web app.

## Requirements

## Parameters
* NAMESPACE: Optional, default 'pyzip-demo', Namespace to deploy the cluster in.
* OPENSHIFT_TARGET: Required, target openshift deployment
* OPENSHIFT_USER: Required, openshift user to login as
* OPENSHIFT_PASS: Required, openshift users password

## Running the application
`docker run -e "OPENSHIFT_TARGET=<openshift_target>" -e "OPENSHIFT_USER=<user>" -e "OPENSHIFT_PASS=<password>" ansibleplaybookbundle/pyzip-demo-apb provision`

## Tearing down the application
`docker run -e "OPENSHIFT_TARGET=<openshift_target>" -e "OPENSHIFT_USER=<user>" -e "OPENSHIFT_PASS=<password>" ansibleplaybookbundle/pyzip-demo-apb deprovision`
