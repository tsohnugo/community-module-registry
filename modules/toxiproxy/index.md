---
title: Toxiproxy
categories:
  - web
docs:
  - id: java
    url: https://java.testcontainers.org/modules/toxiproxy/
    maintainer: core
    example: |
      ```java
      var toxiproxy = new ToxiproxyContainer(DockerImageName.parse("ghcr.io/shopify/toxiproxy:2.12.0"));
      toxiproxy.start();
      ```
    installation: |
      ```xml
      <dependency>
          <groupId>org.testcontainers</groupId>
          <artifactId>toxiproxy</artifactId>
          <version>1.20.0</version>
          <scope>test</scope>
      </dependency>
      ```
  - id: go
    url: https://golang.testcontainers.org/modules/toxiproxy/
    maintainer: core
    example: |
      ```go
      toxiproxyContainer, err := toxiproxy.Run(context.Background(), "ghcr.io/shopify/toxiproxy:2.12.0")
      ```
    installation: |
      ```bash
      go get github.com/testcontainers/testcontainers-go/modules/toxiproxy
      ```
  - id: nodejs
    url: https://node.testcontainers.org/modules/toxiproxy/
    maintainer: core
    example: |
      ```javascript
      const container = await new ToxiProxyContainer("ghcr.io/shopify/toxiproxy:2.12.0").start();
      ```
    installation: |
      ```bash
      npm install @testcontainers/toxiproxy --save-dev
      ```
description: |
  Toxiproxy is a framework for simulating network conditions. It's made specifically to work in testing, CI and development environments, supporting deterministic tampering with connections, but with support for randomized chaos and customization.
---
