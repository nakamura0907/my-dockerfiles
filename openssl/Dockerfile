ARG VARIANT=3.19.1
FROM alpine:${VARIANT}

RUN \
    apk update \
    && apk add --no-cache openssl \
    && rm -rf /var/cache/apk/*


ENTRYPOINT ["openssl"]
