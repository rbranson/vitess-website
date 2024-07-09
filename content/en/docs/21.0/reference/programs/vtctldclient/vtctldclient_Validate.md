---
title: Validate
series: vtctldclient
commit: b9b567acbb1f36404f46b5daa168d37831dd137f
---
## vtctldclient Validate

Validates that all nodes reachable from the global replication graph, as well as all tablets in discoverable cells, are consistent.

```
vtctldclient Validate [--ping-tablets]
```

### Options

```
  -h, --help           help for Validate
  -p, --ping-tablets   Indicates whether all tablets should be pinged during the validation process.
```

### Options inherited from parent commands

```
      --action_timeout duration              timeout to use for the command (default 1h0m0s)
      --compact                              use compact format for otherwise verbose outputs
      --server string                        server to use for the connection (required)
      --topo-global-root string              the path of the global topology data in the global topology server (default "/vitess/global")
      --topo-global-server-address strings   the address of the global topology server(s) (default [localhost:2379])
      --topo-implementation string           the topology implementation to use (default "etcd2")
```

### SEE ALSO

* [vtctldclient](../)	 - Executes a cluster management command on the remote vtctld server.
