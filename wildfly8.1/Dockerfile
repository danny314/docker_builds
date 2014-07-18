#Wildfly 8.1 image

FROM ubuntu

#RUN apt-get update

################## Begin Wildfly Installation ######################
# Create directory 

WORKDIR /opt
#Copy Wildfly
ADD wildfly-8.1.0.Final /opt/wildfly-8.1.0.Final

#Copy Java8
ADD jdk1.8.0 /opt/jdk1.8.0

RUN ls -l


#Download and install from Internet
#ADD http://download.jboss.org/wildfly/8.1.0.Final/wildfly-8.1.0.Final.tar.gz /opt/
#RUN tar -zxf wildfly-8.1.0.Final.tar.gz




# Install java8 from Internet
#RUN apt-get -y install software-properties-common
#run add-apt-repository -y ppa:webupd8team/java
#run apt-get update
#run echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | sudo /usr/bin/debconf-set-selections
#run apt-get install -y oracle-java8-installer

# Expose the default port
EXPOSE 8080
ENV JAVA_HOME /opt/jdk1.8.0
ENTRYPOINT /bin/bash

##################### INSTALLATION END #####################
