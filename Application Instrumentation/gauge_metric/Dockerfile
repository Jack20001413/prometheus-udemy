FROM python:3.9-slim

WORKDIR /app

COPY . /app/

RUN pip3 install --no-cache-dir prometheus_client && \
    pip3 install --no-cache-dir python-dotenv

EXPOSE 5000 5003

ENTRYPOINT [ "python3", "gauge_metric.py" ]