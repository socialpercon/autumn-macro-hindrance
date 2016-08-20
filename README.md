# Autumn Macro Hindrance

Or, how to generate a micro service cluster boilerplate.

## Idea

Use one line of bash to generate a Spring Cloud Netflix based microservice cluster.

## Setup
Please configure the variables in the `./amh` script.

## Building

Run `./amh demo && ./amh build`.

[Please create a bug report if something breaks. =)][1]

## What works
- config-server [using this repo][2]
- Micro Service loading config from config-server


## What does not work
- everything else, this is heavily under construction

[1]: https://github.com/uvwxy/autumn-macro-hindrance/issues
[2]: https://github.com/uvwxy/amh-demo-cluster-config