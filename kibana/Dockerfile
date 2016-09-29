FROM kibana:4.6.1

COPY config/kibana.yml /opt/kibana/config/

RUN kibana plugin --install elastic/sense \
  && kibana plugin --install elastic/timelion

RUN kibana plugin --install kaae -u https://github.com/elasticfence/kaae/releases/download/snapshot/kaae-latest.tar.gz

RUN kibana plugin -i logtrail -u https://github.com/sivasamyk/logtrail/releases/download/0.1.3/logtrail-4.x-0.1.3.tar.gz

RUN kibana plugin -i kibana-time-plugin -u https://github.com/nreese/kibana-time-plugin/archive/master.zip

RUN kibana plugin -i prelert_swimlane_vis -u https://github.com/prelert/kibana-swimlane-vis/archive/v0.1.0.tar.gz

RUN kibana plugin -i tagcloud -u https://github.com/stormpython/tagcloud/archive/master.zip

RUN kibana plugin -i heatmap -u https://github.com/stormpython/heatmap/archive/1.0.0.zip

RUN kibana plugin -i vectormap -u https://github.com/stormpython/vectormap/archive/master.zip

RUN kibana plugin -i kibi_radar_vis -u  https://github.com/sirensolutions/kibi_radar_vis/archive/4.5.3.zip

RUN kibana plugin -i kibi_wordcloud_vis -u https://github.com/sirensolutions/kibi_wordcloud_vis/raw/4.5.3/target/kibi_wordcloud_vis-4.5.3.zip

RUN kibana plugin -i kibi_timeline_vis -u https://github.com/sirensolutions/kibi_timeline_vis/raw/4.5.3/target/kibi_timeline_vis-4.5.3.zip

RUN kibana plugin -i kibana-html-plugin -u https://github.com/raystorm-place/kibana-html-plugin/releases/download/v0.0.3/kibana-html-plugin-v0.0.3.tar.gz

RUN kibana plugin -i kibana-slider-plugin -u https://github.com/raystorm-place/kibana-slider-plugin/releases/download/v0.0.2/kibana-slider-plugin-v0.0.2.tar.gz

RUN kibana plugin -i enhanced_tilemap -u https://github.com/nreese/enhanced_tilemap/archive/master.zip
