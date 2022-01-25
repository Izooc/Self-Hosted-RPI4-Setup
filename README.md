# Self-Hosted-RPI4-Setup
My story of setting up self-hosted apps without portforwarding.
![image](/mockup.png)

# Tailscale
Tailscale was the first thing to spark me to setup my rpi4 self hosted apps.
Essentially, I couldnt portforward due to my router and so i scoured the web for a solution.
I started off by seeing if i could use tailscale to route my pi's traffic to a VPS (Like Digitalocean)
I eventually figured out that if i advertise my Digitalocean VPS as a tailscale exit node, and route my RPI through that, and use nginx proxy manager on my digitalocean vps
to create a proxy host and point it to my raspberry pi's ip.

#Resources I Used
[This Repo](https://github.com/abhilesh/self-hosted_docker_setups) has been amazing. Multiple docker compose files for all your needs.
The Awesome Selfhosted repo has been very useful aswell

