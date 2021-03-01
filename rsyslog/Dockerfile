FROM ubuntu
RUN apt update && apt install -y rsyslog
ADD rsyslog.conf /etc/rsyslog.conf
CMD /etc/init.d/rsyslog restart && tail -f
