FROM russianpostman/api_yamdb_web:latest

WORKDIR /app

COPY requirements.txt .

RUN pip3 install -r requirements.txt --no-cache-dir

COPY .. .

CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ]