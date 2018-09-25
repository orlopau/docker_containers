FROM ubuntu:latest
RUN apt update
RUN apt install -y ffmpeg
WORKDIR /usr/bin
EXPOSE 8090
ADD ffserver.conf /etc/
CMD ["ffserver"]
