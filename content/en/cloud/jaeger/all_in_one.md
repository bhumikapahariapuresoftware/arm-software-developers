---
processors : ["Ubuntu"]
software : ["linux"]
title: "Install Jaeger All-in-one"
type: docs
weight: 1
hide_summary: true
description: >
    Learn how to install Jaeger All-in-one for quick local testing, launches the Jaeger UI, collector, query, and agent, with an in memory storage component..
---

## Prerequisites

* Physical machines or cloud nodes with Ubuntu installed.

## Install Jaeger All-on-one from package

Follow [this documentation](https://www.jaegertracing.io/docs/1.26/getting-started/#all-in-one) to install Jaeger All-in-one.

### Steps in brief

* Deployed Jaeger using the docker image on both the platforms:

```console
docker run -d --name jaeger -e COLLECTOR_ZIPKIN_HOST_PORT=:9411 -p 5775:5775/udp -p 6831:6831/udp -p 6832:6832/udp -p 5778:5778 -p 16686:16686 -p 14268:14268 -p 14250:14250 -p 9411:9411 quay.io/jaegertracing/all-in-one:latest
```

[<-- Return to Learning Path](/content/en/cloud/jaeger/#sections)

