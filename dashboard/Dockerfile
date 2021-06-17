FROM alpine

LABEL maintainer "Lubo"

ADD app.tgz /

RUN apk add python3 py3-pip \
	&& pip3 install uvicorn fastapi jinja2 python-multipart

VOLUME /app/data/

WORKDIR /app

CMD ["/usr/bin/env", "python3", "/app/dashboard.py"]
