FROM jenkins/jenkins:lts

USER root
RUN apt-get update && \
    curl -sL https://deb.nodesource.com/setup_9.x | bash - && \
    apt-get install -y nodejs npm && \
    npm cache verify && \
    npm install n -g && \
    n stable && \
    ln -sf /usr/local/bin/node /usr/bin/node  && \
    apt-get purge -y nodejs npm

USER jenkins