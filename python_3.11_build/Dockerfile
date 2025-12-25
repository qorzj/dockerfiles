FROM python:3.11-slim

RUN apt-get update && apt-get install -y tzdata build-essential libpcre3-dev zlib1g-dev

RUN pip install -U pip
CMD date && python -c "print(__import__('datetime').datetime.now())"
