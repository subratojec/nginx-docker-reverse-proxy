FROM python:3.10-slim

WORKDIR /app

COPY . /app

RUN pip install --no-cache-dir flask && apt update && apt install -y curl 

EXPOSE 8002

CMD ["python", "app.py"]