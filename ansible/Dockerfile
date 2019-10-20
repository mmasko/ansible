FROM ubuntu:19.04
RUN export DEBIAN_FRONTEND="noninteractive" \
&& apt-get update \
&& apt-get install -y --no-install-recommends \
apt-transport-https \
ca-certificates \
gpg-agent \
p7zip \
software-properties-common \
unzip \
wget \
winbind \
&& rm -rf /var/lib/apt/lists/* \
&& add-apt-repository multiverse \
&& dpkg --add-architecture i386 \
&& apt-get update \
&& apt-get install wine-stable winbind xvfb steamcmd
