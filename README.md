# spt-fika
Play Escape from Tarkov with friends on your own Unraid server!

### Current "latest" version
SPT version 3.10.5
Fika v2.3.6

### What's this about?

I deserve no credit. I just take someone else's Dockerfile, create an image, upload it to Dockerhub, and reference it in an Unraid app XML template. This way users can pull the image through Unraids excellent Community Apps plugin.

Originally, I built images using [OnniSarna's guide and Dockerfile](https://github.com/OnniSaarni/SPT-Fika-Docker-Guide), but this hasn't been updated since the SPT team moved to Github as their official repo, and, as of January 5, 2025, it behaves strangely. I have altered it to reference the current SPT repo address, but the Dockerfile continues to generate SPT-Fika server images with SPT 3.10.4 and Fika v2.3.5 *at the latest*, even *if* newer versions are specified in the Dockerfile ARGs.

[Zedramus and contributers have put together a current Dockerfile here](https://github.com/zhliau/fika-spt-server-docker) for the emulated backend server. I am now using this to build images for the Unraid App.

Note: this Git refers only to the emulated server backend. I'll publish a template on Unraid CA for the dedicated client soon, but that requires more setup and know-how, and I must make considerations on how to document and support it!

### How to Connect

To connect, point your SPT Launcher (Settings, enable Developer Mode, fill in the URL field) to the host address (or this container's address if you have it bridged) with the port specified (e.g, http://192.168.1.10:6969, if 192.168.1.10 is your host IP).

### Credit, Links, Etc

Major kudos to [zedramus and his Dockerfile](https://github.com/zhliau/fika-spt-server-docker/blob/master/Dockerfile) and OnniSarna (for his [original guide](https://github.com/OnniSaarni/SPT-Fika-Docker-Guide) to create my first SPT server images). 

For more information about the SPT Escape from Tarkov mod, check out https://sp-tarkov.com/.

For more information about the Fika project, check out https://project-fika.gitbook.io/wiki.
