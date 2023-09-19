FROM python:3.9-slim

WORKDIR /app

COPY . .
RUN pip install -r requirements.txt

EXPOSE 90

CMD ["python","-m","uvicorn", "app:app", "--host", "0.0.0.0", "--port", "90"]
