
# VPN Downloads

A brief description of what this project does and who it's for

* PIA_USER: this is your Private Internet Access username
* PIA_PASS: your Private Internet Access password
* PIA_REGION: choose your Private Internet Access region
* TZ: choose the timezone you want the containers to use
* PUID: this is the Unix user ID of the system user the containers will run as
* PGID: this is the Unix group ID of the system user the containers will run as
* QBT_WEBUI_PORT: the port that the qBittorrent client will be accessed via
* NETWORK_SUBNET: this should be the machine's local IP address, with a zero at the end rather than whatever is assigned

# Running
In the directory where your files are, then run:

```docker-compose up -d```

You can then check them using:

```docker-compose ps```

## Configuring

# qBittorrent
The forwarded port for PIA will be stored in the ./config/guetun/piaportforward.json file
So you can view that to grab the port you need to put into qBittorrent's config (I haven't yet got around to making a script that automates this.

# Other software
All configuration files should be in the ./config directory

## Accessing
You should be able to access using the local IP address and the services's port.
e.g. http://localhost:7474 for autobrr
