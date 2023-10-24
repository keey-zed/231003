# Real-Time Data Analytics with Kafka and Spring Cloud Streams

This project demonstrates how to set up and use Apache Kafka for real-time data analytics, along with Spring Cloud Streams for building various Kafka-based services.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
- [Usage](#usage)
  - [1. Manual Setup](#1-manual-setup)
  - [2. Using Docker](#2-using-docker)
- [Testing with Kafka Tools](#testing-with-kafka-tools)
- [Kafka Services](#kafka-services)
- [Web Application](#web-application)

## Getting Started

To get started with this project, you can follow one of two methods: manual setup or using Docker.

### Prerequisites

- Java Development Kit (JDK)
- Apache Kafka
- Spring Boot and Spring Cloud
- Docker (optional)

## Usage

### 1. Manual Setup

Follow these steps to set up and use the project manually:

1. **Download Kafka**: Download and install Apache Kafka. You can find the installation instructions [here](https://kafka.apache.org/quickstart).

2. **Start Zookeeper**: Start the Zookeeper server. You can do this by running the Zookeeper server script.

3. **Start Kafka Server**: Start the Kafka server. You can do this by running the Kafka server script.

### 2. Using Docker

For a more straightforward setup, you can use Docker. Refer to the [Confluent Kafka Docker Quickstart](https://developer.confluent.io/quickstart/kafka-docker/) guide or watch this [video tutorial](https://www.youtube.com/watch?v=9O1Kuk2xXO8).

1. **Create Docker Compose File**: Create a `docker-compose.yml` file with the necessary configurations.

2. **Start Docker Containers**: Use the appropriate command to start the Docker containers for Zookeeper and Kafka broker.
   ```bash
   docker-compose up -d

## Testing with Kafka Tools

Use `kafka-console-producer` and `kafka-console-consumer` to test your Kafka setup within the Docker environment.

## Kafka Services

Using Kafka and Spring Cloud Streams, this project creates various Kafka services:

- A Kafka service producer via a REST Controller.
- A Kafka service consumer.
- A Kafka service supplier.
- A real-time data analytics stream processing service using Kafka Streams.

## Web Application

The project also includes a web application that displays real-time data analytics results from the Kafka stream processing service.
