FROM python:3.11-slim

RUN apt-get update && apt-get install -y tzdata build-essential linux-headers-generic libpcre3-dev zlib1g-dev curl libjpeg-dev
RUN apt-get install -y libgl1-mesa-glx
RUN apt-get install -y libglib2.0-0

RUN pip install -U pip
#RUN pip install torch
#RUN pip install torchvision
CMD date && python -c "print(__import__('datetime').datetime.now())"
