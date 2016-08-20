# Autumn Macro Hindrance

This is a Hello Micro Service World project. It is a bash script called `./amh that generates projects based on components from [Spring Cloud Netflix][3].
The following components are covered:

- Config: `./amh config-server`
	- Fetches config from configured git [repository][2]
- Eureka: `./amh eureka-server <app-name>`
	- Fetches config from config-server
- Zuul: `./amh zuul-server <app-name>`
	- Fetches config from config-server
	- Reverse proxies micro services
- Simple Micro Service: `./amh micro-service <app-name>`
	- Fetches config from config-server

## Idea / Demo

Use one line of bash to generate a Spring Cloud Netflix based micro service cluster.
To setup the demo run

```
./amh create-demo && ./amh package
```

This will produce

```
#bash> ./amh create-demo && ./amh package
Creating demo-cluster-eureka-server
Creating demo-cluster-config-server
Creating demo-cluster-zuul-server
Creating demo-cluster-service-task1
Creating demo-cluster-service-task2
Creating demo-cluster-service-task3

#
# mvn build output truncated
#
```

## Setup
Please look at the configuration variables in the header of the `./amh` script.

## Building

You can run the demo for quick results, or generate parts manually.
To add an additional micro service run `./amh micro-service my-service`.

[Please create a bug report if something breaks. =)][1]

## What works
- config-server [using the example repo][2]
- eureka
- zuul-server
- micro-service


## What does not work
- everything else, this is still under construction

[1]: https://github.com/uvwxy/autumn-macro-hindrance/issues
[2]: https://github.com/uvwxy/amh-demo-cluster-config
[3]: http://cloud.spring.io/spring-cloud-static/spring-cloud-netflix/1.1.5.RELEASE/