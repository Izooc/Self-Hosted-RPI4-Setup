# Self-Hosted-RPI4-Setup
My story of setting up self-hosted apps without portforwarding.
![image](/mockup.png)

# Tailscale
Tailscale was the first thing to spark me to setup my rpi4 self hosted apps.
Essentially, I couldnt portforward due to my router and so i scoured the web for a solution.
I started off by seeing if i could use tailscale to route my pi's traffic to a VPS (Like Digitalocean)
I eventually figured out that if i advertise my Digitalocean VPS as a tailscale exit node, and route my RPI through that, and use nginx proxy manager on my digitalocean vps
to create a proxy host and point it to my raspberry pi's ip.

# Resources I Used
[This Repo](https://github.com/abhilesh/self-hosted_docker_setups) has been amazing. Multiple docker compose files for all your needs.
The [Awesome Selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) repo has been very useful aswell.
[DBTech's YT Channel](https://www.youtube.com/c/DBTechYT) has been brilliant for setting up fail2ban with cloudflare, Authelia and the likes.

# How?
Essentially i just took the docker compose file from the Self hosted docker setups repo, searched up the config, and edited it to my needs, such as running things off of my usb stick and external hard drive due to a lack of storage on a 16GB Micro SD Card.
