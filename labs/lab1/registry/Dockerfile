FROM registry.access.redhat.com/rhel7
MAINTAINER Student <student@foo.io>

RUN yum --enablerepo rhel-7-server-extras-rpms install docker-registry -y && yum clean all

EXPOSE 5000

ENTRYPOINT ["/usr/bin/registry"]

CMD ["serve", "/etc/docker-distribution/registry/config.yml"]
