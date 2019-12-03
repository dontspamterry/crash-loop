# crash-loop
Simple alpine-based container that sleeps for 5 seconds and then exits. Intent is to produce a CrashLoopBackOff scenario for Prometheus alerting

## Build
```bash
docker build -t <image name> .
```

## Repo
https://hub.docker.com/repository/docker/dontspamterry/crash-loop

## K8S Deploy
kubectl apply -f crash-loop-deployment.yaml --namespace=<namespace>
