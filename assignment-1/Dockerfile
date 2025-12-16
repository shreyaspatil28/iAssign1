FROM python:3.11-slim

WORKDIR /app
COPY index.html .

EXPOSE 7000

CMD ["python", "-m", "http.server", "7000"]
