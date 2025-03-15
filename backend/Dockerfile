FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

COPY src/testsite /app/testsite

EXPOSE 8000

CMD ["uvicorn", "testsite.main:app", "--host", "0.0.0.0", "--port", "8000"]