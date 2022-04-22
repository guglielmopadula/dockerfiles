# syntax=docker/dockerfile:1
	
FROM python:3.9.2

WORKDIR /data

COPY test.txt requirements.txt
RUN apt-get update
RUN apt-get -y install graphviz pandoc nbconvert* texlive-xetex texlive-fonts-recommended texlive-plain-generic
RUN pip3 install -r requirements.txt

CMD ["jupyter", "lab", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
