FROM python:3.8

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY src/ /app
WORKDIR /app

CMD [ "uvicorn", "app:app", "--host", "0.0.0.0", "--port", "15400" ]