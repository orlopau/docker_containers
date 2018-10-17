FROM openjdk:8
WORKDIR /home/
EXPOSE 1990
RUN apt-get update && apt-get -y install apt-transport-https
RUN sh -c 'echo "deb https://packages.atlassian.com/atlassian-sdk-deb stable contrib" >>/etc/apt/sources.list' && \
	wget https://packages.atlassian.com/api/gpg/key/public && \    
	apt-key add public && \
	apt-get update && apt-get install -y atlassian-plugin-sdk
RUN groupadd -g 1000 confi && \
	useradd -m -u 1000 -g confi confi
USER confi
CMD echo Use docker run or docker exec /bin/bash to use the sdk

