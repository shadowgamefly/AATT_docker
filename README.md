# AATT_docker
Automated testing tools using docker based on AATT.

## Set up
1. Have docker installed
```sh
$ git clone https://github.com/shadowgamefly/AATT_docker.git
$ cd AATT_docker
$ docker-compose build
$ docker-compose up
```

## Runtime
Here is a sample ajax script which would initiate the request:

``` html
var xmlhttp = new XMLHttpRequest();
xmlhttp.open("POST","http://localhost:3000/evaluate",true);
xmlhttp.setRequestHeader("Content-type","application/x-www-form-urlencoded");
xmlhttp.send("source=" + document.getElementsByTagName('html')[0].value + "&output=json";
```

Then the result should showup in both docker log as well as *xmlhttp.response*

A better UI interface can also be accessed through http://localhost:3000

## link

Thanks to [Paypal AATT](https://github.com/paypal/AATT).
