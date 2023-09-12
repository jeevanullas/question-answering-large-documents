FROM public.ecr.aws/lts/ubuntu:20.04

RUN apt-get update
RUN apt-get -y install python3-pip
COPY requirements.txt /app/requirements.txt
RUN pip3 install -r /app/requirements.txt

COPY ./* ./app/
WORKDIR /app/

EXPOSE 5000

CMD ["python3", "app.py"]
