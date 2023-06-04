---
share: true
---
I managed to configure my own git server for Obsidian. The trickiest bit was configuring it so that it's accessible via HTTP, since the Obsidian Git client on mobile/tablet doesn't work over SSH.

I did it! This article should really be expanded but the gist of it is:

* Create a repo on my nas (`git init --bare`)
* Make my nas accessible via Tailscale
* Install nginx + fcgiwrap + git in a docker image running on my synology
* Profit

It took me a while. I dump here some of the references that I used:

https://www.wundertech.net/how-to-use-docker-on-a-synology-nas/
https://esc.sh/blog/setting-up-a-git-http-server-with-nginx/
https://registry.hub.docker.com/_/nginx/

To access my nas remotely I use [[Tailscale]] 