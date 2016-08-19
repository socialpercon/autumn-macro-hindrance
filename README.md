# Autumn Macro Hindrance

Or, how to generate a micro service cluster boilerplate.

## Idea

Use one line of bash to generate a Spring Cloud Netflix based microservice cluster.

## Setup
Please configure the variables in the `./amh` script.

## Building

Run `./amh demo && ./amh build`.

Please create a bug report if something breaks. =)

## What works
- config-server (don't forget the config repo)
    - add task1.yml and task2.yml (Seting server.port: 9001/9002, and so on)
- Micro Service loading config from config-server


## What does not work
- everything else, this is heavly under construction
