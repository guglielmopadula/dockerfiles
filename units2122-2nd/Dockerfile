# syntax=docker/dockerfile:1

FROM python:3.9.2

WORKDIR /app

COPY test.txt requirements.txt
RUN pip3 install -r requirements.txt

CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
