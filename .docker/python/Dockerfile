FROM python:3.9.6-alpine3.14
RUN apk update && apk upgrade
RUN pip install flask twilio

COPY server.py ./var/www/html/
COPY config.py ./var/www/html/


ENTRYPOINT [ "python", "/var/www/html/server.py" ]