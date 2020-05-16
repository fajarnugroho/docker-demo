FROM python:3.7

RUN apt-get update && apt install -y dumb-init
WORKDIR /app
COPY requirements.txt /app/requirements.txt

RUN pip install -r requirements.txt && rm -rf /root/.cache
COPY . /app
ENTRYPOINT ["/usr/bin/dumb-init", "--"]
CMD ["python", "hello.py"]
