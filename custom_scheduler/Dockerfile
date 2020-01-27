FROM ubuntu:18.04

RUN apt-get update && \
    apt-get install -y python3-pip

RUN pip3 install --upgrade pip==9.0.1

COPY requirements.txt .
COPY sched.py .
RUN pip3 install -r requirements.txt

CMD ["python3","sched.py"]