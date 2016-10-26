# Strongswan on Docker

Base docker image to run a Strongswan IPsec and a XL2TPD server.

## Usage

Run the following to start the container:

```
docker run -d -p 500:500/udp -p 4500:4500/udp -p 1701:1701/udp --privileged --name psk -e VPN_PSK=<public shared key> -e VPN_USER=<your name> -e VPN_PASSWORD=<your passward> wyvern/strongswan
```
