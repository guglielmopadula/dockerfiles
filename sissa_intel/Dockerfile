# syntax=docker/dockerfile:1
	
FROM intel/oneapi-aikit:2022.1.2-devel-ubuntu18.04

WORKDIR /data
ENV DEBIAN_FRONTEND=noninteractive 
RUN apt-get update
COPY conda.txt requirements.txt
RUN conda config --append channels conda-forge
RUN conda install -y --file requirements.txt


CMD ["jupyter", "lab", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
