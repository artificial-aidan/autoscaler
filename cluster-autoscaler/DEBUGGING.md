VScode settings

```
    "configurations": [
        {
            "name": "Connect to server",
            "type": "go",
            "request": "attach",
            "mode": "remote",
            "substitutePath": [
                {
                    "from": "${workspaceFolder}/",
                    "to": "/gopath/src/k8s.io/autoscaler/",
                },
            ],
            "port": 40000,
            "host": "127.0.0.1",
            "trace":"verbose",
            "apiVersion": 2
        },
```

## Building

`make build-in-docker`
`make make-image`
`docker tag staging-k8s.gcr.io/cluster-autoscaler-amd64:dev reg.notartificial.xyz:1443/artificial/cluster-autoscaler:aidan2`
