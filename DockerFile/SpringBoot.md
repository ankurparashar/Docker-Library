#### SpringBoot DockerFile Template
```
FROM java:8

VOLUME /tmp

ARG DATA_PATH=/src/main/resources

EXPOSE 8080

COPY ${DATA_PATH}/predefined_data/ /mnt/data/predefined_data/
COPY ${DATA_PATH}/docker-init.sh /mnt/data/docker-init.sh
COPY ${DATA_PATH}/newrelic/ /mnt/data/newrelic/

ADD /build/libs/my-api-1.0.jar my-api-1.0.jar
```
