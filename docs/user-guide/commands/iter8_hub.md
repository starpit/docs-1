---
template: main.html
title: "Iter8 Hub"
hide:
- toc
---
## iter8 hub

Download experiment chart

### Synopsis


Download an experiment chart to a local directory.

	$ iter8 hub -c load-test-http

This command is intended for development and testing of experiment charts. For production usage, the iter8 launch command is recommended.


```
iter8 hub [flags]
```

### Options

```
      --gitFolder string   Git folder containing iter8 charts (default "github.com/iter8-tools/iter8.git?ref=v0.10.5//charts")
  -h, --help               help for hub
```

### Options inherited from parent commands

```
  -l, --loglevel string   trace, debug, info, warning, error, fatal, panic (default "info")
```

### SEE ALSO

* [iter8](iter8.md)	 - Kubernetes release optimizer

###### Auto generated by spf13/cobra on 14-Apr-2022
