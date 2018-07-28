# Multicontainer example on resin.io

This example is an multicontainer example built on 3 Resin examples
- multicontainer-getting-started: https://github.com/resin-io-projects/multicontainer-getting-started.git
- resin-wifi-connect: https://github.com/resin-io/resin-wifi-connect.git
- simple-server-node:https://github.com/resin-io-projects/simple-server-node.git
- Some ideas how to build docker compose.yml from: resin-wifi-connect-api - https://github.com/resin-io-projects/resin-wifi-connect-api.git

The idea was to have a portable demo to bring to different locations with different WiFi SSID and to get it running without having to re-flash for each SSID. 

The example will run wifi connect and if a known network can be attached it just skips. If no known network can be found it will startup as a WiFi hotspot and you can connect to it and configure WiFi. It then has a simple we server. 
- once you have selected a WiFi NW (SSID & Password provisioned via wifi connect), it will use that SSID on next power-off-on cycle. Good for deplyments as well . 
