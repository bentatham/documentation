# Ruby
This is the ruby language plugin for Gauge.

It contains a launcher component (gauge-ruby.go) written in golang which is used to start the plugin from gauge.

Build from Source
-----------------

### Requirements
* [Golang](http://golang.org/)
* [Ruby](https://www.ruby-lang.org/en/)
* [Gauge](http://getgauge.io)


###Compiling

````
go run make.go
````

For cross platform compilation (launcher)

````
go run make.go --all-platforms
````

###Installing

After compiling

````
go run make.go --install
````

Installing to a CUSTOM_LOCATION

````
go run make.go --install --plugin-prefix CUSTOM_LOCATION
````

###Creating distributable


Note: Run after compiling

````
go run make.go --distro
````

For distributable across platforms os, windows and linux for bith x86 and x86_64

````
go run make.go --distro --all-platforms
````

New distribution details need to be updated in the ruby-install.json file in  [gauge plugin repository](https://github.com/getgauge/gauge-repository) for a new verison update.
