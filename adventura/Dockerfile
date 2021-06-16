FROM python:alpine
LABEL maintainer="Lubo"

ADD https://github.com/obulobul/python-textovka/archive/refs/heads/main.zip /

RUN adduser -G users -H -D -g "the player" player \ 
	&& unzip main.zip \
	&& mkdir app \
	&& mv /python-textovka-main/* /app \
	&& rm -rf main.zip python-textovka-main

WORKDIR /app/

USER player

CMD [ "/usr/bin/env", "python3", "game.py" ]
