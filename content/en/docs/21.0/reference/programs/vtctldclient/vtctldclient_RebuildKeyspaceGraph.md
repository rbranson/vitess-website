---
title: RebuildKeyspaceGraph
series: vtctldclient
commit: b9b567acbb1f36404f46b5daa168d37831dd137f
---
## vtctldclient RebuildKeyspaceGraph

Rebuilds the serving data for the keyspace(s). This command may trigger an update to all connected clients.

```
vtctldclient RebuildKeyspaceGraph [--cells=c1,c2,...] [--allow-partial] ks1 [ks2 ...]
```

### Options

```
      --allow-partial   Specifies whether a SNAPSHOT keyspace is allowed to serve with an incomplete set of shards. Ignored for all other types of keyspaces.
  -c, --cells strings   Specifies a comma-separated list of cells to update.
  -h, --help            help for RebuildKeyspaceGraph
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
