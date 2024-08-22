FROM python:3.11-slim

RUN apt-get update && apt-get install -y tzdata build-essential linux-headers-generic libpcre3-dev zlib1g-dev curl libjpeg-dev

RUN pip install -U pip
RUN pip install torch
RUN pip install torchvision
CMD date && python -c "print(__import__('datetime').datetime.now())"