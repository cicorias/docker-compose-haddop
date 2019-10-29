FROM cicorias/hadoop-base

MAINTAINER Shawn Cicoria <github@cicoria.com>

# COPY WordCount.jar /opt/hadoop/applications/WordCount.jar
COPY missingcard-1.0-SNAPSHOT.jar /opt/hadoop/applications/missingcard-1.0-SNAPSHOT.jar

ENV JAR_FILEPATH="/opt/hadoop/applications/missingcard-1.0-SNAPSHOT.jar"
ENV CLASS_TO_RUN="WordCount"
ENV PARAMS="/input /output"

ADD run.sh /run.sh
RUN chmod a+x /run.sh

CMD ["/run.sh"]
