FROM python:3.7-alpine
LABEL maintainer="Josip Naletilic"

WORKDIR .

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

EXPOSE 5000

COPY . .
ENTRYPOINT [ "python", "app/consumer.py" ]