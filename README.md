# stcache
A simple cache server showing how to use hashicorp/raft

1.  start first node. 
```
   bash run.sh 1 1
```

2.  start second node. 
```
   bash run.sh 2 0
```

3.  start third node. 
```
   bash run.sh 3 0
```

## write to cluster
curl "http://127.0.0.1:6000/set?key=ping&value=pong"

## read from cluster
curl "http://127.0.0.1:6000/get?key=ping"

