FROM debian

RUN apt-get update
RUN apt-get install -y gawk python3 wget unzip xxd

WORKDIR "/build"
ENTRYPOINT ["./build.sh"]
