# mock-real-time-data-stream-with-python-and-kafka
Make a mock “real-time” data stream with Python and Kafka
https://towardsdatascience.com/make-a-mock-real-time-stream-of-data-with-python-and-kafka-7e5e23123582

**Start kafka**
```
cd c:/kafka
bin\windows\zookeeper-server-start.bat config/zookeeper.properties
```

```
cd c:/kafka
bin\windows\kafka-server-start.bat config/server.properties
```

**Start the consumer**
```
python bin/processStream.py my-stream
```

**Start the producer**
```
python bin/sendStream.py data/data.csv my-stream
```
