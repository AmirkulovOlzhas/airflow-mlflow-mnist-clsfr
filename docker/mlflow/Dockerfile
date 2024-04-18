FROM python:3.12.2

WORKDIR /mlflow

COPY requirements.txt /tmp

RUN pip install -r /tmp/requirements.txt

ENV BACKEND_URI sqlite:///mlflow.db

EXPOSE 5000

CMD mlflow ui --backend-store-uri $BACKEND_URI --host 0.0.0.0