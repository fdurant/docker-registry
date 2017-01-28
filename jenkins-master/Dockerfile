# Inspired by
# https://engineering.riotgames.com/news/putting-jenkins-docker-container
# https://engineering.riotgames.com/news/docker-jenkins-data-persists
# https://engineering.riotgames.com/news/jenkins-docker-proxies-and-compose

FROM jenkins:1.609.1
MAINTAINER Frederik Durant

USER root
RUN mkdir /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins
USER jenkins

ENV JAVA_OPTS="-Xmx8192m"
ENV JENKINS_OPTS="--handlerCountStartup=100 --handlerCountMax=300 --logfile=/var/log/jenkins/jenkins.log"

CMD ["echo", "Jenkins: May I help you, sir?"]
