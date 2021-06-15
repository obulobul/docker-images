FROM scratch
LABEL maintainer="Lubo"
LABEL homepage="https://github.com/obulobul"
ADD alpine-minirootfs-3.13.5-x86_64.tar.gz /
RUN apk add cmatrix
LABEL description="Matrix!"
CMD ["/usr/bin/cmatrix"]
