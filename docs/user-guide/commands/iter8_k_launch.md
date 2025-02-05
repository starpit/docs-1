---
template: main.html
title: "Iter8 K Launch"
hide:
- toc
---
## iter8 k launch

Launch an experiment in Kubernetes

### Synopsis


Launch an experiment in Kubernetes. 

	$ iter8 k launch -c load-test-http --set url=https://httpbin.org/get

To locally render the Kubernetes experiment, use the dry option.

	$ iter8 k launch -c load-test-http \
	  --set url=https://httpbin.org/get \
	  --dry

By default, the current directory is used to download and unpack the experiment chart. Change this location using the destDir option.

	$ iter8 k launch -c load-test-http \
	  --set url=https://httpbin.org/get \
	  --destDir /tmp


```
iter8 k launch [flags]
```

### Options

```
  -c, --chartName string         name of the experiment chart
      --chartsParentDir string   directory under which the charts folder is located (default ".")
      --dry                      simulate an experiment launch
      --gitFolder string         Git folder containing iter8 charts (default "github.com/iter8-tools/iter8.git?ref=v0.10.5//charts")
  -g, --group string             name of the experiment group (default "default")
  -h, --help                     help for launch
      --noDownload               reuse local charts dir; do not download from Git
      --set stringArray          set values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2)
      --set-file stringArray     set values from respective files specified via the command line (can specify multiple or separate values with commas: key1=path1,key2=path2)
      --set-string stringArray   set STRING values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2)
  -f, --values strings           specify values in a YAML file or a URL (can specify multiple)
```

### Options inherited from parent commands

```
      --kube-apiserver string       the address and the port for the Kubernetes API server
      --kube-as-group stringArray   group to impersonate for the operation, this flag can be repeated to specify multiple groups.
      --kube-as-user string         username to impersonate for the operation
      --kube-ca-file string         the certificate authority file for the Kubernetes API server connection
      --kube-context string         name of the kubeconfig context to use
      --kube-token string           bearer token used for authentication
      --kubeconfig string           path to the kubeconfig file
  -l, --loglevel string             trace, debug, info, warning, error, fatal, panic (default "info")
  -n, --namespace string            namespace scope for this request
```

### SEE ALSO

* [iter8 k](iter8_k.md)	 - Work with Kubernetes experiments

###### Auto generated by spf13/cobra on 14-Apr-2022
