FROM alpine:latest
ADD https://raw.githubusercontent.com/nZEDb/nZEDb/0.x/misc/sphinxsearch/sphinx.conf /etc/sphinx/sphinx.conf
RUN apk --update add sphinx \
	&& mkdir -p /var/lib/sphinxsearch \
	&& mkdir -p /var/lib/sphinxsearch/data \
	&& mkdir -p /var/log/sphinxsearch \
	&& mkdir -p /var/run/sphinxsearch \
EXPOSE 9306 9312
CMD searchd --nodetach
