#### Which of the following statements about VMs and Docker containers are not valid?
```
a. Virtual Machine contains the entire Operating System.
b. Docker containers use the resource of the host operating system.
c. Docker containers are used when multiple applications need to run on the same host.
d. Virtual Machine and Docker Containers are the same thing.
```

#### Which of the following are true about Container creation from docker image?
```
a. Each Docker container is assigned a universally unique identifier (UUID).
b. Container creation, Docker allows us to set container names using the name flag.
c. If you do not specify the Container name, docker supplies a randomly-generated name from two words, joined by an underscore.
```

#### Which of the following are advantages of Container Orchestration?
```
a. Scaling up or removing containers to spread application load
b. Movement of containers from one resource to another
c. Load balancing of service discovery between containers
d. Health monitoring of containers and hosts
```

#### Choose the correct statements for the following command. — — — — — “docker image prune”
```
a. command allows us to clean up unused images.
b. By default, the above command will only clean up dangling images.
c. Dangling Images are Image without Tags and Image not referenced by any container
d. All of the above
```

#### Which of the following is not a valid docker CLI command?
```
a. docker image build
b. docker image history
c. docker image import
d. docker image inspect
e. docker image delete
```

#### What is the default Network Type in Docker?
```
a. bridge
b. host
c. overlay
d. macvlan
```

#### Which of the following is not a valid Docker Instruction?
```
a. FROM
b. RUN
c. CMD
d. LABEL
e. ADJUST
```

Which of the following is not a valid docker CLI command?
```
a. docker image build
b. docker image history
c. docker image import
d. docker image inspect
e. docker image delete
```

#### Choose the incorrect statements from the following.
```
a. Multiple containers can be started using the same image.
b. Docker Image is immutable
c. Docker Container has a Top Layer which is writable
d. Docker Container and Docker Images are the same thing
```

#### Which of the following flag is not valid while using HEALTHCHECK instruction?
```
a. interval=DURATION
b. timeout=DURATION
c. start-period=DURATION
d. retries=N (default: 3)
e. All are valid
```

#### Pick the default docker container restart policy.
```
a. none
b. always
c. on-failure
d. unless-stopped
```

#### Which of the following commands are correct?
```
a. docker exec -it service-a bash
b. docker run -it service-a sh
c. docker run — env VAR1=value1 — env VAR2=value2 ubuntu env
d. All of the above.
```

#### Which of the following namespace is not enabled by default?
```
a. volume
b. network
c. pid
d. user
```

#### What is the difference between below commands?
```
docker rmi $(docker images -a — filter=dangling=true -q)
docker rmi $(docker images -f dangling=true -q)
```

##### Which of the following instructions will optimise the size of the image and why?
```
Instruction 1::

ADD https://mysite.com/abc.tar /mnt/data
RUN tar -xJf /mnt/data/abc.tar /mnt/data
RUN make -C /mnt/data all

Instruction 2::

RUN mkdir -p /mnt/data \
&& curl -SL https://mysite.com/abc.tar \
| tar -xJf /mnt/data \
&& make -C /mnt/data all
```

#### Which of the following are true about Docker Secrets?
```
a. Secret can be modified
b. Secret can only be excited on docker-swarm management console
c. Can’t renamed or update to docker secret
```
