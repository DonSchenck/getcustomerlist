# getcustomerlist
Returns a list of customers from a PostgreSQL database


oc new-app https://github.com/donschenck/getcustomerlist --labels=app.kubernetes.io/part-of=customers,systemname=customers,tier=dataaccess,language=nodejs,customers=dataaccess

oc set env deploy/getcustomerlist PG_PORT=5432 PG_HOST=customersdb PG_USER=customersdb PG_PASSWORD=customersdb PG_DATABASE=customersdb