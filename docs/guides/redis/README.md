---
title: Redis
menu:
  docs_{{ .version }}:
    identifier: rd-readme-redis
    name: Redis
    parent: rd-redis-guides
    weight: 10
menu_name: docs_{{ .version }}
section_menu_id: guides
url: /docs/{{ .version }}/guides/redis/
aliases:
  - /docs/{{ .version }}/guides/redis/README/
---

> New to KubeDB? Please start [here](/docs/README.md).

## Supported Redis Features

| Features                         | Availability |
| -------------------------------- | :----------: |
| Clustering                       |   &#10003;   |
| Instant Backup                   |   &#10007;   |
| Scheduled Backup                 |   &#10007;   |
| Persistent Volume                |   &#10003;   |
| Initialize using Snapshot        |   &#10007;   |
| Initialize using Script          |   &#10007;   |
| Custom Configuration             |   &#10003;   |
| Using Custom docker image        |   &#10003;   |
| Builtin Prometheus Discovery     |   &#10003;   |
| Using Prometheus operator |   &#10003;   |

## Life Cycle of a Redis Object

<p align="center">
  <img alt="lifecycle"  src="/docs/images/redis/redis-lifecycle.svg">
</p>

## Supported Redis Versions

| KubeDB Version | Redis:4.0.6 | Redis:5.0.3 |
| :------------: | :---------: | :---------: |
| 0.1.0 - 0.7.0  |  &#10007;   |  &#10007;   |
|     0.8.0      |  &#10003;   |  &#10007;   |
|     0.9.0      |  &#10003;   |  &#10007;   |
|     0.10.0     |  &#10003;   |  &#10003;   |
|     0.11.0     |  &#10003;   |  &#10003;   |
|     0.12.0     |  &#10003;   |  &#10003;   |
|  v0.13.0-rc.0  |  &#10003;   |  &#10003;   |

## Supported RedisVersion CRD

Here, &#10003; means supported and &#10007; means deprecated.

|   NAME   | VERSION  | KubeDB: 0.9.0 | KubeDB: 0.10.0 | KubeDB: 0.11.0 | KubeDB: 0.12.0 | KubeDB: v0.13.0-rc.0 |
| :------: | :------: | :-----------: | :------------: | :------------: | :------------: | :------------------: |
|    4     |    4     |   &#10007;    |    &#10007;    |    &#10007;    |    &#10007;    |       &#10007;       |
|   4-v1   |    4     |   &#10003;    |    &#10007;    |    &#10007;    |    &#10007;    |       &#10007;       |
|   4.0    |   4.0    |   &#10007;    |    &#10007;    |    &#10007;    |    &#10007;    |       &#10007;       |
|  4.0-v1  |   4.0    |   &#10003;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
|  4.0-v2  |   4.0    |   &#10007;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
|  4.0.6   |  4.0.6   |   &#10007;    |    &#10007;    |    &#10007;    |    &#10007;    |       &#10007;       |
| 4.0.6-v1 |  4.0.6   |   &#10003;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
| 4.0.6-v2 |  4.0.6   |   &#10007;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
|  4.0.11  |  4.0.11  |   &#10007;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
|   5.0    |   5.0    |   &#10003;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
|  5.0-v1  |  5.0-v1  |   &#10007;    |    &#10007;    |    &#10003;    |    &#10003;    |       &#10003;       |
|  5.0.3   |  5.0.3   |   &#10003;    |    &#10003;    |    &#10003;    |    &#10003;    |       &#10003;       |
| 5.0.3-v1 | 5.0.3-v1 |   &#10007;    |    &#10007;    |    &#10003;    |    &#10003;    |       &#10003;       |

## User Guide

- [Quickstart Redis](/docs/guides/redis/quickstart/quickstart.md) with KubeDB Operator.
- [Deploy Redis Cluster](/docs/guides/redis/clustering/redis-cluster.md) using KubeDB.
- Monitor your Redis server with KubeDB using [out-of-the-box Prometheus operator](/docs/guides/redis/monitoring/using-prometheus-operator.md).
- Monitor your Redis server with KubeDB using [out-of-the-box builtin-Prometheus](/docs/guides/redis/monitoring/using-builtin-prometheus.md).
- Use [private Docker registry](/docs/guides/redis/private-registry/using-private-registry.md) to deploy Redis with KubeDB.
- Use [kubedb cli](/docs/guides/redis/cli/cli.md) to manage databases like kubectl for Kubernetes.
- Detail concepts of [Redis object](/docs/guides/redis/concepts/redis.md).
- Detail concepts of [RedisVersion object](/docs/guides/redis/concepts/catalog.md).
- Want to hack on KubeDB? Check our [contribution guidelines](/docs/CONTRIBUTING.md).
