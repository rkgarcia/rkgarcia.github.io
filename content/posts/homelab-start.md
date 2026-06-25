---
date: 2026-06-25T11:41:43-06:00
# description: ""
# image: ""
lastmod: 2026-06-25
showTableOfContents: false
# tags: ["",]
title: "Homelab Start"
type: "post"
---
I'm currently working in my home lab. If you know about many tools with the same purpose, it creates a problem to choose the right tool that fits your current or near-future requirements.

At this time, the stack is:
* Proxmox to mount all.
* Vaultwarden for password management.
* Immich is used as a photo backup for my family's devices.
* Caddy as a proxy to present all apps with SSL and a custom URL for each app.
* AdGuard is used as our DNS for home devices, and it rewrites DNS queries to resolve names locally for apps.
* Tailscale to connect all devices without internet exposure.

All apps are running over Proxmox using LXC.
The apps are accessible using application.my.domain over HTTPS.
At home, you access directly; out of home, you only require a Tailscale connection.


*Next steps:*

* NAS, using a TrueNAS in a VM with storage hardware passthrough.
* CVS solution, my options are Gitlab or Forgejo (I always use GitLab, but I want to try something new, Forgejo looks lightweight and is written in GoLang)
* CI/CD solution. If I choose GitLab, it has embedded, but my option with Forgejo is Woodpecker.
* For multimedia, Jellyfin and Plex are my options. I don't know any other tools.


I want my home lab to work as a production-ready infrastructure!


What do you think? What do you do in your home labs?