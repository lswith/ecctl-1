## ecctl deployment elasticsearch restart

Restarts an Elasticsearch cluster

### Synopsis

Restarts an Elasticsearch cluster

```
ecctl deployment elasticsearch restart <cluster id> [flags]
```

### Options

```
  -h, --help                            help for restart
      --rolling-by-name                 Performs the restart in a rolling fashion (one instance at a time)
      --rolling-by-zone                 Performs the restart in a rolling fashion (one logical zone at a time)
      --shard-init-wait-time duration   Time to wait for shards that show no progress of initializing, before rolling the next group (default 10m0s)
      --skip-snapshot                   Prevents snapshotting prior to restart
  -t, --track                           Tracks the progress of the performed task
```

### Options inherited from parent commands

```
      --apikey string      API key to use to authenticate (If empty will look for EC_APIKEY environment variable)
      --config string      Config name, used to have multiple configs in $HOME/.ecctl/<env> (default "config")
      --force              Do not ask for confirmation
      --format string      Formats the output using a Go template
      --host string        Base URL to use
      --insecure           Skips all TLS validation
      --message string     A message to set on cluster operation
      --output string      Output format [text|json] (default "text")
      --pass string        Password to use to authenticate (If empty will look for EC_PASS environment variable)
      --pprof              Enables pprofing and saves the profile to pprof-20060102150405
  -q, --quiet              Suppresses the configuration file used for the run, if any
      --timeout duration   Timeout to use on all HTTP calls (default 30s)
      --trace              Enables tracing saves the trace to trace-20060102150405
      --user string        Username to use to authenticate (If empty will look for EC_USER environment variable)
      --verbose            Enable verbose mode
```

### SEE ALSO

* [ecctl deployment elasticsearch](ecctl_deployment_elasticsearch.md)	 - Manages Elasticsearch clusters

