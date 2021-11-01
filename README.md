# JMeter AMQP Plugin

A [JMeter](http://jmeter.apache.org/) plugin to publish & consume messages from [RabbitMQ](http://www.rabbitmq.com/) or any [AMQP](http://www.amqp.org/) message broker.

## Overview

//TODO

## Installation

1. Download the [latest release](https://github.com/aliesbelik/jmeter-amqp-plugin/releases/latest) or [build your own](#build) from the source code.
2. Put `jmeter-amqp-plugin-VERSION-jar-with-dependencies.jar` into `$JMETER_HOME/lib/ext` directory.\
It contains the necessary AMQP client dependency, no other jars are required.
3. Restart JMeter GUI.

In case if you need the plugin without the AMQP client included, you can use the `jmeter-amqp-plugin-VERSION.jar`,
but you have to ensure that the [RabbitMQ client library](https://www.rabbitmq.com/java-client.html) - `amqp-client-VERSION.jar` - is installed in `$JMETER_HOME/lib` directory.

## Usage

This plugin includes 2 samplers:

- **AMQP Publisher**
- **AMQP Consumer**

![amqp-plugin-samplers](docs/images/amqp-plugin-samplers.png)

A pre-configured example scenario can be found in the [examples](docs/examples) directory.

## Build

### Build requirements

In order to build JMeter AMQP plugin from source, you will need:

- [Java 8](https://www.oracle.com/downloads/)
- [Apache Maven 3](https://maven.apache.org/)

Build dependencies are managed by Maven.\
Jars should automatically be downloaded by Maven as part of the build process.

In addition, you'll need to copy or symlink the following from `$JMETER_HOME/lib/ext` directory:

- ApacheJMeter_core.jar

### Build from source

To build, just execute:

```
mvn clean package
```

This will create 2 jars in `/target` directory, the original jar and the jar with all the dependencies within (this is the one you need):

```
target/jmeter-amqp-plugin-VERSION.jar
target/jmeter-amqp-plugin-VERSION-jar-with-dependencies.jar
```

To install, execute:

```
cp target/jmeter-amqp-plugin-VERSION-jar-with-dependencies.jar $JMETER_HOME/lib/ext
```

## Contributing

Contributions are welcome.
