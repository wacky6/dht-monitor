dht-monitor
===



## Install
1. Install [bcm2835](http://www.airspayce.com/mikem/bcm2835/index.html), used to control Pi's GPIO

2. `npm -g i wacky6/dht-monitor`



## Usage
```
  Usage: dht-monitor [options] <gpio>

  Options:
    -h, --help             output usage information
    -V, --version          output the version number
    -i, --interval <secs>  Read interval, in seconds; min: 3, default: 5
    -a, --aggregate        Aggregate readings, report timeseries as changes
    -h, --db-host <host>   Rethinkdb host to report readings
    -t, --tag <tag>        Tag for database record, default: os.hostname()
    --db-port <port>       Rethinkdb port, default: 28015
    --db <db>              Rethinkdb database, default: "sensor"
    --table <table>        Rethinkdb table, default: "dht"
    -w, --warmup <secs>    Warpup delay, in seconds; default: 5
```



## LICENSE
MIT
