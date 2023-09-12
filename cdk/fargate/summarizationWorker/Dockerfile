FROM public.ecr.aws/lts/ubuntu:20.04

RUN apt-get update
RUN apt-get -y install python3-pip
COPY requirements.txt /opt/requirements.txt
RUN pip3 install -r /opt/requirements.txt 

COPY app.py /opt/app.py

CMD ["/usr/bin/python3", "/opt/app.py"]

