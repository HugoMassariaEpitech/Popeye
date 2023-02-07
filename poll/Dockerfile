FROM python:3.9.16-slim

WORKDIR /app/poll

COPY . .

RUN pip3 install -r requirements.txt

EXPOSE 80

CMD ["python3", "app.py"]