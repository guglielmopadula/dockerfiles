# syntax=docker/dockerfile:1
	
FROM python:3.8.13

WORKDIR /data
ENV DEBIAN_FRONTEND=noninteractive 
RUN apt-get update
COPY conda.txt requirements.txt
RUN pip install -r requirements.txt


CMD ["jupyter", "lab", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
