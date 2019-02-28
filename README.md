# my-docker-containers
A set of my docker containers and how to manage them.

All my services are running behind Traefik - The Cloud Native Edge Router (https://traefik.io).

## Traefik - The Cloud Native Edge Router
Traefik makes it very easy to set up ssl secured services on a docker host. Just set a name on your dns pointing to your server, start the docker container and you are set.

  * Traefik is: a reverse proxy / load balancer that's easy, dynamic, automatic, fast, full-featured, open source, production proven, provides metrics, and integrates with every major cluster technology

It is running on my host network so it can manage dockerized services and host based services. In my configuration (traefik.toml.example) you see 'cockpit' as such host based service.

## Tvheadend
I am using Tvheadend for receiving iptv from my internet provider and distributing it in my flat to my TVs. What Tvheadend is writing on https://tvheadend.org about itself:

  * Tvheadend is a TV streaming server and recorder for Linux, FreeBSD and Android supporting DVB-S, DVB-S2, DVB-C, DVB-T, ATSC, ISDB-T, IPTV, SAT>IP and HDHomeRun as input sources.
  * Tvheadend offers the HTTP (VLC, MPlayer), HTSP (Kodi, Movian) and SAT>IP streaming.
  * Multiple EPG sources are supported (over-the-air DVB and ATSC including OpenTV DVB extensions, XMLTV, PyXML).
  * The code is hosted at github https://github.com/tvheadend/tvheadend

I am running Tvheadend on the host network so it is able to receive the iptv multicast packets.
