FROM ubuntu:bionic

RUN apt-get update && \
	apt-get install -y openjdk-8-jdk && \
	apt-get clean
	
RUN java -version

COPY /target/$jarToCopy /app/app.jar

CMD ["java", "-cp", "/app/app.jar", "com.examples.hellodocker.App"]
