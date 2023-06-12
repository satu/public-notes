---
share: true
---
I use [Tailscale](https://tailscale.com/) to access my local network when I'm on the road, and to also control some remote machine easily.

Use cases
* accessing my NAS from phones / tablets. This includes accessing the  [Personal Git server for Obsidian](Personal%20Git%20server%20for%20Obsidian.md)
* routing all the traffic via my home connection (using exit nodes), for example to watch UK TV or Sky when I'm abroad
* have guaranteed access to a remote Raspberry Pi running in Italy, which I use as a bridge if I want to watch Italian TV. For performance reason, the actual bridge is done with a (vanilla) Wireguard direct tunnel between that box and my router, but I still keep Tailscale as a reliable way to access the machine

Limitations
* Unfortunately tailscale is banned on my corporate laptop. I have to rely on my phone/tablet when I'm not home.

TODO
* [ ] document the Wireguard tunnel solution