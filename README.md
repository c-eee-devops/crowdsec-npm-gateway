# Nginx Proxy Manager Configuration With Croudsec

## Requiurements

- A little bit of Docker experience

- For this guide, I will be utilizing a portainer instance that has already been configured using Docker.

- A domain that already points to your old Nginx proxy manager instance (which I assume you configured with a database)

## Setting Up Nginx Proxy Manager

First, we will need to set up Nginx Proxy Manager via its `docker compose`

I will be using baudneo fork because we will need to use that fork later anyway. Make sure that you set your database passwords to something else.

you will also need to run the following before you run `docker compose up -d`

```
mkdir /Nginx-Proxy-Manger
```
```
touch /Nginx-Proxy-Manger/crowdsec-openresty-bouncer.conf
```
