---
title: InfluxDB
categories:
  - relational-database
docs:
  - id: java
    url: https://java.testcontainers.org/modules/databases/influxdb/
    maintainer: core
    example: |
      ```java
      var influx = new InfluxDBContainer<>(DockerImageName.parse("influxdb:2.0.7"));
      influx.start();
      ```
    installation: |
      ```xml
      <dependency>
          <groupId>org.testcontainers</groupId>
          <artifactId>influxdb</artifactId>
          <version>1.20.0</version>
          <scope>test</scope>
      </dependency>
      ```
  - id: go
    url: https://golang.testcontainers.org/modules/influxdb/
    maintainer: core
    example: |
      ```go
      influxdbContainer, err := influxdb.Run(context.Background(), "influxdb:1.8.10")
      ```
    installation: |
      ```bash
      go get github.com/testcontainers/testcontainers-go/modules/influxdb
      ```
  - id: dotnet
    url: https://www.nuget.org/packages/Testcontainers.InfluxDb
    maintainer: core
    example: |
      ```csharp
      var influxDbContainer = new InfluxDbBuilder()
        .WithImage("influxdb:2.7")
        .Build();
      await influxDbContainer.StartAsync();
      ```
    installation: |
      ```bash
      dotnet add package Testcontainers.InfluxDb
      ```
  - id: python
    url: https://testcontainers-python.readthedocs.io/en/latest/modules/influxdb/README.html
    maintainer: core
    example: |
      ```python
      with InfluxDbContainer() as influxdb_container:
          connection_url = influxdb_container.get_url()
      ```
    installation: |
      ```bash
      pip install testcontainers[influxdb]
      ```
description: |
  InfluxDB is an open-source time series database for storage and retrieval of time series data in fields such as operations monitoring, application metrics, Internet of Things sensor data, and real-time analytics.
---
