#### pkmasredis
#####cp4 Programming redis
Redis serialization protocol(RESP)
#####cp6 scaling
######Apporaches
three ways for partitioning data with redis: client-side partitioning, proxy assisted partitioning,query routing(current impl of redis cluster)
```
BITCOUNT partition
GETBIT partition 80000
```
```
DBSIZE
```
```
SET book:1 "1"
SET book:2 "2"
CLUSTER KEYSLOT book:1
CLUSTER KEYSLOT book:2
```
```
MSET {book}:1 "1" {book}:2 "2"
```
