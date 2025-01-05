# spt-fika
Play Escape from Tarkov with friends on your own private server!

I deserve no credit. All I did was take someone else's Dockerfile, create an image and reference it in an Unraid app XML template. This way users can pull the image through Unraids excellent Community Apps "shop."

Originally, I built images using [OnniSarna's guide and Dockerfile](https://github.com/OnniSaarni/SPT-Fika-Docker-Guide), but this hasn't been updated since the SPT team moved to Github as their official repo and, as of today, the Dockerfile continues to generate SPT-Fika server images on SPT 3.10.4 and Fika v2.3.5, even *if* newer versions are specified in the Dockerfile ARGs.

[Zedramus and contributers have put together a current Dockerfile here](https://github.com/zhliau/fika-spt-server-docker) for both the emulated backend server, and which I have used to build images for this Unraid App.

Note: this Git refers only to the emulated server backend. I'll publish a template on Unraid CA for the dedicated client soon, but that requires more setup and know-how, and I must make considerations on how to document and support it!

As for this piece, on first run, allow a few minutes for the image to generate necesary server files and import the database. You can watch the logs to see when it's ready to accept connections.

To connect, point your SPT Launcher (Settings, enable Developer Mode, fill in the URL field) to the host address (or this container's address if you have it bridged) with the port specified (e.g, http://192.168.1.10:6969, if 192.168.1.10 is your host IP).

Major kudos to [zedramus and his Dockerfile](https://github.com/zhliau/fika-spt-server-docker/blob/master/Dockerfile) and OnniSarna (for his [original guide](https://github.com/OnniSaarni/SPT-Fika-Docker-Guide) to create my first SPT server images). 

For more information about the SPT Escape from Tarkov mod, check out https://sp-tarkov.com/.

For more information about the Fika project, check out https://github.com/project-fika/Fika-Documentation.
