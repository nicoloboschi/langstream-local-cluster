# Langstream Local Cluster

## Get started

```
curl -Ls "https://raw.githubusercontent.com/nicoloboschi/langstream-local-cluster/main/get-llc.sh" | bash
```

## Start the cluster

```
$ llc start
Minikube: ✅
Minio: ✅
LangStream: ✅
Kafka: ✅
Config updated: webServiceUrl=http://127.0.0.1:64136
Config updated: apiGatewayUrl=http://127.0.0.1:64141
Config updated: tenant=default
CLI: ✅
Ready 🚀
```

## Start a cluster using local images

```
cd $langstream_root_dir
llc start --dev
```

## Stop the cluster

```
llc delete
```

## Get help

```
LangStream local cluster.

Syntax: ./llc [options]

Options:
  start [--dev] [--load]    Start the LangStream local cluster.
                            --dev    Start in development mode. This will use the latest development images that are built locally.
                            --load   Load LangStream images instead of building them. Only for dev mode.
  delete                    Delete the LangStream local cluster.
  langstream|cli <command>  Run the LangStream CLI with the given command.
  load <image>              Load a specific Docker image into Minikube.
  build <component>         Build docker image for a specific LangStream component and restart it. No arguments to rebuild all the images.
  get-instance              Get the path to the LangStream app instance YAML file.
  get-config                Get the path to the Kubernetes configuration file.
  kubectl <command>         Run kubectl with the given command.
  k9s <command>             Run K9s with the given command.
  help                      Print this help message. 
```
