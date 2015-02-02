# Proxy

nodejs proxy to be used in case many services are bounded to one host.
It uses virtual hosting to route to backends.


### Setup

Edit server.js, change ROUTER const to your need

### Run it

    # cd /files/apps
    # git clone https://github.com/redpelicans/proxy.git
    # <do setup>
    # docker run -d --restart=always --link website:website --link ghost:ghost  --name proxy -p 80:80 -v "/files/apps/proxy":/usr/src/web -w /usr/src/web  redpelicans/website sh run

