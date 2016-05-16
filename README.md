Containerized 32bit Firefox for WebEx
===================

This Ubuntu based Docker container is an attempt to get a reasonably stable environment to run WebEx on Linux. 

Use the included ``run.sh`` to start the container, as there are several commandline arguments needed for this to run properly.
Example usage: ``./run.sh <webex link>`` where webex link may look like https://abcdef.webex.com/vwxyz/j.php?MTID=xxxxxxxxxxxxxxxxxxxxxxx

**Note:** Since WebEx is a SaaS application, it can change at any time, so this container may or may not work sometimes. In my own testing I've found that sometimes the screen sharing doesn't always work, receiving nor sending, but it might have to do with my desktop environment (i3wm with gnome-panel). TP enabled WebEx sessions are not supported at all on Linux, so these won't work with this container either.

The image currently includes only the minimal packages needed to run WebEx on Linux: firefox:i386, openjdk-7-jre:i386, icedtea-7-plugin:i386, and some X11 support libs.

See this on GitHub: https://github.com/mbessler/ff32-webex
See this on DockerHub: https://hub.docker.com/r/mbessler/ff32-webex

Pull-requests welcome.
