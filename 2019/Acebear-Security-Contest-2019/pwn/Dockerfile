FROM ubuntu:18.04

MAINTAINER anonymous
RUN apt-get update

RUN apt-get install netcat -y

RUN apt-get install -y python-pip python-dev build-essential

RUN pip install -I subprocess32==3.5.0rc1

RUN pip install flask

RUN mkdir /tmp/data

RUN chmod -R 777 /tmp/data

RUN useradd -m gifremake

COPY ./app /app

RUN chown -R root:root /app
RUN chmod -R 755 /app

COPY ./flag /home/gifremake/flag
COPY ./gifremake /home/gifremake/gifremake

COPY ./init.sh /init.sh

RUN chmod +x /init.sh
RUN chmod +x /home/gifremake/gifremake

RUN chown -R root:gifremake /home/gifremake
RUN chmod -R 755 /home/gifremake
RUN chmod 640 /home/gifremake/flag

WORKDIR /app

CMD ["/init.sh"]

EXPOSE 8080
