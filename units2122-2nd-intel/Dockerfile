# syntax=docker/dockerfile:1
	
FROM intel/oneapi-aikit:2022.1.2-devel-ubuntu18.04

WORKDIR /data

COPY conda.txt requirements.txt
RUN apt-get update
RUN apt-get -y install graphviz
RUN conda config --append channels conda-forge
RUN conda config --append channels fico-xpress
RUN conda install -y --file requirements.txt
RUN pip3 install pyro-ppl==1.3.0

CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
