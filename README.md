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
llc dev start
```

## Stop the cluster

```
llc delete
```

## Get help

```
llc help
```
