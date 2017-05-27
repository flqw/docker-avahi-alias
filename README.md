# docker-avahi-alias
mdns/avahi cnames with docker

# Usage
Uses the host dbus socket to add avahi cname records.
```
docker run -d -v /var/run/dbus/system_bus_socket:/var/run/dbus/system_bus_socket flqw/avahi-alias:latest \
[hostname.local] [hostname2.local] [hostname3.local] ...
```

Taken from https://gist.github.com/gdamjan/3168336 with a few fixes and put into a docker image.
