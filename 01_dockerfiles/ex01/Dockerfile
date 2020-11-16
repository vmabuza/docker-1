FROM		debian

ENV			TS3SERVER_LICENSE=accept
		

RUN			apt-get update && apt-get upgrade -y
		

RUN			apt-get install -y wget bzip2
		

RUN			wget http://dl.4players.de/ts/releases/3.0.13.4/teamspeak3-server_freebsd_amd64-3.0.13.4.tar.bz2
		

RUN			tar -xvf teamspeak3-server_freebsd_amd64-3.0.13.4.tar.bz2
		

WORKDIR			teamspeak3-server_freebsd_amd64
		

ENTRYPOINT		sh ts3serer_minimal_runscript.sh


#docker build -t ex01 .
#docker run -p 9987:9987/udp -p 10011:10011 -p 30033:30033 -e TS3SERVER_LICENSE=accept teamspeak
