FROM node:6
MAINTAINER SOUMYA
RUN mkdir -p /usr/src/app
WORKDIR  /usr/src/app
COPY package.json /usr/src/app
RUN npm cache clean
RUN npm install

COPY . /usr/src/app
RUN node db.js
ENTRYPOINT ["npm"]
CMD ["start"]

