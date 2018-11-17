# Snap for the transmission-daemon BitTorrent client

[![Build status](https://img.shields.io/travis/albertodonato/transmission-daemon-snap.svg)](https://travis-ci.com/albertodonato/tramisssion-daemon-snap)


This snap contains the [Transmission](https://transmissionbt.com) daemon, along
with some CLI tools.

After installing the snap the service web interface will be accessible at
<http::/localhost:9091> by default.

This can be changed via

```bash
    snap set transmission-daemon port=<new-port>
```

When using `transmission-daemon.remote`, it will be automatically pointed at
the local server, so no host/port configuration should be passed.


## Build the snap

The snap can be built by simply running:

```bash
    snapcraft
```

Once, built, install the snap with:

```bash
    sudo snap install --dangerous transmission-daemon_*.snap
```
