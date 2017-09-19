FROM ubuntu:16.04

#Install.
RUN \
	sed -i 's/archive.ubuntu.com/mirrors.aliyuncs.com/g' /etc/apt/sources.list && \
	apt-get update && \
	apt-get install -y software-properties-common && \
	add-apt-repository ppa:webupd8team/java && \
	apt-get update && \
	echo debconf shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
	echo debconf shared/accepted-oracle-license-v1-1 seen true | debconf-set-selections && \
	apt-get install -y oracle-java8-installer

CMD ["bash"]