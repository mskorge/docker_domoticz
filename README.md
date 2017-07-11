Domoticz
======

Domoticz - http://www.domoticz.com/

Latest Domoticz git release forked from sdesbure/domoticz
https://hub.docker.com/r/sdesbure/domoticz/

##How to use

**Pull image**

```
docker pull skorge/domoticz

```

**Run container**

```
docker run -d -p 8080:8080 --name=<container name> -v <path for config files>:/config -v /etc/localtime:/etc/localtime:ro --device=<device_id> skorge/domoticz
```

Please replace all user variables in the above command defined by <> with the correct values (you can have several USB devices attached, just add other `--device=<device_id>`).

**Access Domoticz**

```
http://<host ip>:8080
```

8080 can be another port (you change `-p 8080:8080` to `-p 8081:8080` to have 8081 out of the container for example).
