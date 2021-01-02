FROM alpine:3.7

RUN apk add --no-cache python3 jpeg && \
    apk add --no-cache --virtual .build-deps gcc python3-dev zlib-dev jpeg-dev linux-headers musl-dev
RUN  CFLAGS="-fcommon" pip3 install --no-cache-dir rpi.gpio
RUN  pip3 install --no-cache-dir luma.oled psutil
RUN apk del .build-deps

