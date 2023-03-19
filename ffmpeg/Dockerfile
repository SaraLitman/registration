ARG BASE_IMAGE_TAG=latest
FROM ubuntu:${BASE_IMAGE_TAG}

RUN apt-get update \
 && apt-get install -y --no-install-recommends ffmpeg=6.0 \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*


ENTRYPOINT ["ffmpeg"]