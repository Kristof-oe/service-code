FROM python:3.13-slim 

COPY --from=ghcr.io/astral-sh/uv:0.11 /uv /bin/

WORKDIR /app

COPY . .

RUN uv sync

EXPOSE 8000

CMD ["uv", "run", "app.py"]
