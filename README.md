health-data-svc
=======

## Description

Simple API for access data on health providers

## Install

* npm install

## Run

```
node index.js
```

or

```
heroku local web
```

##REST API Calls
GET http://localhost:5000/providers?max_discharges=12&min_discharges=6&max_average_covered_charges=50000.00&min_average_covered_charges=10000.00&min_average_medicare_payments=6000&max_average_medicare_payments=7000&state=WA

##Data Notes:
1.  some minor preprocessing of data to replace " " w/ "_"
2.  Used the postgres 'money' type which is a little different from other databases
3.

##Notes
1.