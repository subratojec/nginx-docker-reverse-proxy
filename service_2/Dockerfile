FROM python:3.13-slim

WORKDIR /app

RUN pip install --no-cache-dir uv

COPY . /app

# RUN uv sync --frozen

RUN apt update && apt install -y curl && rm -rf /var/lib/apt/lists/*

EXPOSE 8002

CMD ["uv", "run", "python", "app.py"]