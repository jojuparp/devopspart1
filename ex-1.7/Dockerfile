FROM ubuntu:16.04

WORKDIR /usr/app
RUN apt-get update && apt-get install -y curl

RUN echo '"Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;' > skripti.sh
RUN chmod +x ./skripti.sh

CMD ["/bin/sh", "skripti.sh"]