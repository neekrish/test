FROM openjdk:8u121-jdk
COPY mygit/jetty-http2-server-example.jar /usr/bin/myapp/jetty-http2-server-example.jar
COPY mygit/alpn-boot-8.1.11.v20170118.jar /usr/bin/myapp/alpn-boot-8.1.11.v20170118.jar
COPY mygit/dependencies/ /usr/bin/myapp/dependencies
WORKDIR /usr/bin/myapp
EXPOSE 8443
CMD java -Xms1024m -Xmx1024m -Xbootclasspath/p:alpn-boot-8.1.11.v20170118.jar -jar jetty-http2-server-example.jar