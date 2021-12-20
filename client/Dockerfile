FROM python:3.8

ENV LANG=C.UTF-8
ENV LC_ALL=C.UTF-8
ENV PIP_NO_CACHE_DIR=off

WORKDIR /usr/src/physmem2profit

RUN apt-get update && \
    apt-get install -y python3-dev gcc git python3-pip virtualenv libncurses5-dev fuse

COPY . .

RUN pip install -r requirements.txt

ENTRYPOINT [ "python /usr/src/physmem2profit" ]