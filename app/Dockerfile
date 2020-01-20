#FROM node:4-onbuild
FROM node:6
MAINTAINER Bryan CS <yanser25@gmail.com>

ADD . /var/www/srv

WORKDIR /var/www/srv

RUN npm install
RUN chmod +x ./test/test.sh
RUN ./test/test.sh

CMD ["nodejs", "app.js"]
