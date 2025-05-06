---
title: GaussDB
categories:
  - relational-database
docs:
  - id: java
    url: https://java.testcontainers.org/modules/databases/gaussdb/
    maintainer: core
    example: |
      ```java
      var gaussdb = new GaussDBContainer<>(DockerImageName.parse("opengauss/opengauss:7.0.0-RC1.B023"));
      gaussdb.start();
      ```
    installation: |
      ```xml
      <dependency>
          <groupId>org.testcontainers</groupId>
          <artifactId>gaussdb</artifactId>
          <version>1.20.0</version>
          <scope>test</scope>
      </dependency>
      ```
description: |
  GaussDB is a trustworthy data foundation for mission-critical workloads, where high availability, performance, security, scalability, and intelligence are non-negotiable and OpenGauss is the community version for GaussDB.
---
