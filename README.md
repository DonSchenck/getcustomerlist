# getcustomerlist
Returns a list of customers from a PostgreSQL database

## Part of the Red Hat Developer learning path entitled "Using Red Hat OpenShift labels"

oc new-app https://github.com/redhat-developer-demos/getcustomerlist --labels=app.kubernetes.io/part-of=customers,systemname=customers,tier=dataaccess,language=nodejs,customers=dataaccess

oc set env deploy/getcustomerlist PG_PORT=5432 PG_HOST=customersdb PG_USER=customersdb PG_PASSWORD=customersdb PG_DATABASE=customersdb