FROM anapsix/alpine-java:8_jdk

RUN wget -O mvn.tar.gz http://www.us.apache.org/dist/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz &&\
tar xzvf mvn.tar.gz &&\
mv apache-maven-3.6.3 mvn &&\
rm mvn.tar.gz &&\
mkdir /app

WORKDIR /app

CMD ["/mvn/bin/mvn", "spring-boot:run"]

EXPOSE 8080