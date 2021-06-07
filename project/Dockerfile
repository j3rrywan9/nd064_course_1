FROM python:2.7

RUN apt-get update && apt-get install -y lsof

COPY techtrends /app
WORKDIR /app
RUN pip install -r requirements.txt

CMD ["python init_db.py"]

EXPOSE 3111

CMD ["python", "app.py"]
