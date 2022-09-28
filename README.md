
# Portainer Docker setup
A Portainer + Caddy with automatic SSL setup for production using docker swarm.

## Guide

Clone this repository.

Go into the directory containing your project (`<project-name>`), and start the app in production mode:

```
SERVER_NAME=your-domain-name.example.com \
docker stack deploy -c docker-compose.yml portainer
```

Be sure to replace `your-domain-name.example.com` with your actual domain name.

Your server is up and running, and a Let's Encrypt HTTPS certificate has been automatically generated for you.
Go to `https://your-domain-name.example.com` and enjoy!



