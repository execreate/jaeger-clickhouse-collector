# Jaeger collector w/ Clickhouse storage backend

## Overview

This is a docker-compose setup that runs Jaeger collector query service with Clickhouse backend using
[jaeger-clickhouse plugin v0.13.0](https://github.com/jaegertracing/jaeger-clickhouse/releases/tag/0.13.0).
The [oauth2-proxy (v7.2.1.linux-amd64)](https://github.com/oauth2-proxy/oauth2-proxy/releases/tag/v7.2.1)
is used to secure the Jaeger UI.

## Prerequisites

- Docker
- Docker compose

## Running

Make sure to edit the [oauth2_proxy config file](oauth2-proxy/proxy.env) to match your environment then run:

```bash
docker-compose up -d
```
