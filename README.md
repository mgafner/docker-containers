# my-docker-containers
A set of my docker containers and how to manage them.

All my services are running behind Traefik - The Cloud Native Edge Router (https://traefik.io).

## Tvheadend
I am using Tvheadend for receiving iptv from my internet provider and distributing it in my flat to my TVs. What Tvheadend is writing on https://tvheadend.org about itself:

  * Tvheadend is a TV streaming server and recorder for Linux, FreeBSD and Android supporting DVB-S, DVB-S2, DVB-C, DVB-T, ATSC, ISDB-T, IPTV, SAT>IP and HDHomeRun as input sources.
  * Tvheadend offers the HTTP (VLC, MPlayer), HTSP (Kodi, Movian) and SAT>IP streaming.
  * Multiple EPG sources are supported (over-the-air DVB and ATSC including OpenTV DVB extensions, XMLTV, PyXML).
  * The code is hosted at github https://github.com/tvheadend/tvheadend

I am running Tvheadend on the host network so it is able to receive the iptv multicast packets.
