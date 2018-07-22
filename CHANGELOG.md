# Changelog

## v6.13

- Ring got new options called `HashReplicas` and `Hash`. It is recommended to set `HashReplicas = 1000` for better keys distribution between shards.
- Cluster client was optimized to use much less memory when reloading cluster state.

## v6.12

- ClusterClient got new option called `ClusterSlots` which allows to build cluster of normal Redis Servers that don't have cluster mode enabled. See https://godoc.org/github.com/go-redis/redis#example-NewClusterClient--ManualSetup