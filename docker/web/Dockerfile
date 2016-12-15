FROM tomcat:8-jre8
MAINTAINER Alex Mcknight <mcknight816@gmail.com>

RUN echo "export JAVA_OPTS=\"-Dapp.env=staging\"" > /usr/local/tomcat/bin/setenv.sh

ADD tomcat-users.xml /usr/local/tomcat/conf/
ADD martialarts.jdbc.properties /usr/local/tomcat/temp/MartialArts/
ADD app.properties /usr/local/tomcat/temp/MartialArts/
ADD MartialArts.war /usr/local/tomcat/webapps

CMD ["catalina.sh", "run"]