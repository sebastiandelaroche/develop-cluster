FROM jenkins/jenkins:latest

# Distributed Builds plugins
RUN /usr/local/bin/install-plugins.sh ssh-slaves

# UI
RUN /usr/local/bin/install-plugins.sh greenballs
RUN /usr/local/bin/install-plugins.sh simple-theme-plugin

# install Maven
USER root
RUN apt-get update && apt-get install -y maven
USER jenkins