FROM ubuntu:14.04

#Install.
RUN \
	sed -i 's/archive.ubuntu.com/mirrors.163.com/g' /etc/apt/sources.list && \
	apt-get update && \
	apt-get install -y build-essential && \
	apt-get install -y software-properties-common

CMD ["bash"]


