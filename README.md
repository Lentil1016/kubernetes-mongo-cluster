# kubernetes-mongo-cluster

- HA cluster
- with 3 shard
- official mongo image only
- single yaml file bootup
- for kubernetes

```
$ kubectl apply -f https://github.com/Lentil1016/kubernetes-mongo-cluster/raw/master/mongo.yaml

# The job mongo-bootup will boot up the cluster
$ kubectl logs mongo-bootup-9tlxs
Initializating configuration nodes
Successed [ "ok" : 1, ]
Initializing mongosh1
Successed [{ "ok" : 1  }]
Initializing mongosh2
Successed [{ "ok" : 1  }]
Initializing mongosh3
Successed [{ "ok" : 1  }]
Adding rs1 to cluster
Successed [ "ok" : 1, ]
Adding rs2 to cluster
Successed [ "ok" : 1, ]
Adding rs3 to cluster
Successed [ "ok" : 1, ]
Mongo cluster ready
```
