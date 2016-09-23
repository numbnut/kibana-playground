FROM kibana:4.6.1

COPY config/kibana.yml /opt/kibana/config/

RUN kibana plugin --install elastic/sense \
  && kibana plugin --install elastic/timelion
