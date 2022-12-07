#### Python DockerFile Template
```
FROM python:3.6

RUN apt-get update

COPY requirements.txt ./
RUN pip install -r requirements.txt
COPY . .

WORKDIR .

## Expose the docker port
EXPOSE 8000

## Initiate the Server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
```
