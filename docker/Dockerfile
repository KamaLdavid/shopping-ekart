FROM openjdk:8u151-jdk-alpine3.7

EXPOSE 8070

RUN apt-get update && apt-get install -y curl


ENV APP_HOME /usr/src/app

COPY target/shopping-cart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

WORKDIR $APP_HOME

ENTRYPOINT exec java -jar app.jar
