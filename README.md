# Point-to-Point Tunneling Protocol
The Point-to-Point Tunneling Protocol (PPTP) is a method for implementing virtual private networks. PPTP uses a control channel over TCP and a GRE tunnel operating to encapsulate PPP packets.

## Requirement:
- docker version > 1.9
- 1723 port is open for docker host

## Usage:
git clone this repo
```
git clone https://github.com/hotsun/docker-pptpd ~/docker-pptpd
```

Update/Create new user
```
cd ~/docker-pptpd
vi chap-secrets
```

Use docker compose to run it
```
docker-compose -f pptpd.yml up -d
```
