FROM eclipse-temurin:17-jdk-alpine

# mc-image-helper installieren
RUN apk add --no-cache curl bash
RUN curl -sLo /usr/local/bin/mc-image-helper \
    https://github.com/itzg/mc-image-helper/releases/latest/download/mc-image-helper \
    && chmod +x /usr/local/bin/mc-image-helper

COPY run.sh /run.sh
RUN chmod +x /run.sh

CMD ["/run.sh"]
