FROM ubuntu:14.04
MAINTAINER Darrin Wortlehock <darrin@beyondthestory.com>

ENV HOME /root

ADD . /build

RUN /build/prepare.sh && \
	/build/system_services.sh && \
	/build/utilities.sh && \
	/build/cleanup.sh

CMD ["/sbin/my_init"]
