FROM maven:alpine

ARG APP_DIR=app
WORKDIR ${APP_DIR}
COPY .. .

RUN mvn clean package

EXPOSE 8182

RUN ls
RUN pwd

ENTRYPOINT ["java"]
CMD ["-jar", "./target/service-a-0.0.1.jar"]