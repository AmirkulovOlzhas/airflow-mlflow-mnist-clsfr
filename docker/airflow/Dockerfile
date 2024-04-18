FROM apache/airflow:2.9.0

RUN pip install -U pip --upgrade pip

COPY requirements.txt /tmp

RUN pip install --no-cache-dir -r /tmp/requirements.txt