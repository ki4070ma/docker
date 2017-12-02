FROM jenkins/jenkins:lts

USER root
RUN apt-get update
RUN curl -sL https://deb.nodesource.com/setup_9.x | bash -
RUN apt-get install -y nodejs npm
RUN npm cache verify
RUN npm install n -g
RUN n stable
RUN ln -sf /usr/local/bin/node /usr/bin/node
RUN apt-get purge -y nodejs npm

USER jenkins