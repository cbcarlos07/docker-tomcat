FROM tomcat:latest
ADD ./bs-service-dsv2.war /usr/local/tomcat/webapps/app.war
EXPOSE 8080
RUN sh -c 'touch /usr/local/tomcat/webapps/app.war'
ENTRYPOINT [ "sh","-c","java -Djava.security.egd=file:/dev/./urandom -jar /usr/local/tomcat/webapps/app.war" ]
CMD ["catalina.sh", "run"]
