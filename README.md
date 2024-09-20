FROM python:3-alpine

LABEL name Discern
LABEL src "https://github.com/0xKaran/Discern"
LABEL creator 0xKaran
LABEL desc "Fast SSRF hunter."

RUN apk add git && git clone https://github.com/0xKaran/Discern.git Discern
WORKDIR Discern
