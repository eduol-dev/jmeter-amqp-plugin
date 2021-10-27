# JMeter AMQP Plugin

A [JMeter](http://jmeter.apache.org/) plugin to publish & consume messages from [RabbitMQ](http://www.rabbitmq.com/) or any [AMQP](http://www.amqp.org/) message broker.

## Overview

//TODO

## Installation

To install the plugin, build the project and copy the generated **jmeter-amqp-plugin-VERSION-jar-with-dependencies.jar** from `target/dist` to `$JMETER_HOME/lib/ext` directory, then restart JMeter GUI.
It contains the necessary AMQP client dependency, no other jars are required.

In case if you need the plugin without the AMQP client included, you can use the **jmeter-amqp-plugin-VERSION.jar**, but you have to ensure that the [RabbitMQ client library](https://www.rabbitmq.com/java-client.html) - **amqp-client-VERSION.jar** - is installed in `$JMETER_HOME/lib` directory.

## Usage

//TODO

## Build

### Build requirements

Build dependencies are managed by Maven.\
JARs should automatically be downloaded by Maven as part of the build process.

In addition, you'll need to copy or symlink the following from `$JMETER_HOME/lib/ext` directory:
* ApacheJMeter_core.jar

### Build from source

The project is built using Maven.\
To execute the build script, just execute:

```
mvn clean package
```

## Contributing

Contributions are welcome.
