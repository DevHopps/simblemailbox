# syntax=docker/dockerfile:1
FROM alpine:latest

#Add Dependencies
RUN apk add --no-cache postfix && \
    rm -rf /var/cache/apk/*

COPY --chmod=+x run.sh /run.sh

EXPOSE 25

RUN ls /

CMD ["sh" "/run.sh"]