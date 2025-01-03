# spt-fika
Play Escape from Tarkov with friends on your own private server!

This is a docker image for the backend server component of Single Player Tarkov (SPT) with the option to install Fika multiplayer mod. I put this together for the Unraid Community Apps ecosystem and Unraid docker templates for convenience and ease-of-use. This image *does not* contain the dedicated client, though I encourage you to check out [zedramus's elegant solution](https://github.com/zhliau/fika-headless-docker).

On first run, allow a few minutes for the image to generate necesary server files and import the database. You can watch the logs to see when it's ready to accept connections.

To connect, point your SPT Launcher (Settings, enable Developer Mode, fill in the URL field) to the host address (or this container's address if you have it bridged) with the port specified (e.g, http://192.168.1.10:6969, if 192.168.1.10 is your host IP).

Major kudos to [zedramus and his Dockerfile](https://github.com/zhliau/fika-spt-server-docker/blob/master/Dockerfile) and OnniSarna (for his [original guide](https://github.com/OnniSaarni/SPT-Fika-Docker-Guide) to create my first SPT server images). 

For more information about the SPT Escape from Tarkov mod, check out https://sp-tarkov.com/.

For more information about the Fika project, check out https://github.com/project-fika/Fika-Documentation.
