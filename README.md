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

###Local:
GET http://localhost:5000/providers?max_discharges=12&min_discharges=6&max_average_covered_charges=50000.00&min_average_covered_charges=10000.00&min_average_medicare_payments=6000&max_average_medicare_payments=7000&state=WA

###Heroku
https://protected-woodland-13807.herokuapp.com/providers?max_discharges=12&min_discharges=6&max_average_covered_charges=50000.00&min_average_covered_charges=10000.00&min_average_medicare_payments=6000&max_average_medicare_payments=7000&state=WA

##Data Notes:
1.  some minor preprocessing of data to replace " " w/ "_"
2.  Used the postgres 'money' type which is a little different from other databases

##Notes
1.  Not a lot of error handling in place since trying to do this fast
2.  Would add some more unit tests
3.  Not heavily tested