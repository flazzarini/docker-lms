# Docker Container for Logitech Media Server

This is a auto-updating docker image to run a Logitech MediaServer or otherwise
known as SqueezeboxServer.

Run Directly:

    docker run -d \
               -p 9000:9000 \
               -p 3483:3483 \
               -p 3483:3483/udp \
               -v <local-state-dir>:/srv/squeezebox \
               -v <audio-dir>:/srv/music \
               flazzarini/docker-lms
