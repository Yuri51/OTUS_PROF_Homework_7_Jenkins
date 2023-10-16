FROM jenkins/agent
USER root
RUN mkdir -p /opt/maven
RUN curl -LSso /var/tmp/apache-maven-3.8.8-bin.tar.gz https://apache.org/dist/maven/maven-3/3.8.8/binaries/apache-maven-3.8.8-bin.tar.gz
RUN tar xzvf /var/tmp/apache-maven-3.8.8-bin.tar.gz -C /opt/maven --strip-components=1
RUN rm /var/tmp/apache-maven-3.8.8-bin.tar.gz
RUN update-alternatives --install /usr/bin/mvn mvn /opt/maven/bin/mvn 10000
RUN mkdir -p /root/.m2
	
