


# Prepare Environment

�b�����Ұ� Rabbit MQ (for windows)

```
docker run --rm -d --name rabbitmq -p 15672:15672 -p 5672:5672 micdenny/rabbitmq-windows
```

�Ұ� N �� Client �����O
```
for /L %i in (1,1,10) do start /min MQRPC.Client\bin\debug\MQRPC.Client.exe
```


�Ұ� M �� Server �����O
```
for /L %i in (1,1,10) do start /min MQRPC.Server\bin\debug\MQRPC.Server.exe
```