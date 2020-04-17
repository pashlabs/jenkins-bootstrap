# https://github.com/jenkinsci/docker-inbound-agent

#export JENKINS_SECRET=??

FROM jenkins/jnlp-slave

ENV JENKINS_URL http://jenkins_master:8080  
ENV JENKINS_SECRET ${JENKINS_SECRET}
ENV JENKINS_AGENT_NAME slave
ENV JENKINS_AGENT_WORKDIR /var/jenkins_home
