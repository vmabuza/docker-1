# docker-1
All day devops (ADDO)



Install Docker Machine

Download the Docker Machine binary and extract it to your PATH (doc)
If you are running macOS:

base=https://github.com/docker/machine/releases/download/v0.16.0 &&
  curl -L $base/docker-machine-$(uname -s)-$(uname -m) >/usr/local/bin/docker-machine &&
  chmod +x /usr/local/bin/docker-machine

If you are running Linux:

base=https://github.com/docker/machine/releases/download/v0.16.0 &&
  curl -L $base/docker-machine-$(uname -s)-$(uname -m) >/tmp/docker-machine &&
  sudo mv /tmp/docker-machine /usr/local/bin/docker-machine &&
  chmod +x /usr/local/bin/docker-machine

Check the installation by displaying the Machine version:

$ docker-machine version
docker-machine version 0.16.0, build 9371605

