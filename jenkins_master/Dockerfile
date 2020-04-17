# https://github.com/jenkinsci/docker/blob/master/README.md
FROM jenkins/jenkins:lts

# Skip initial setup
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false


COPY templates/plugins.txt /usr/share/jenkins/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/plugins.txt
USER root
RUN apt-get update \
    && apt-get install -qqy apt-transport-https ca-certificates curl gnupg2 software-properties-common
USER jenkins