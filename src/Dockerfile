# Use an official Python runtime as a parent image
FROM python:3.11-slim-buster

WORKDIR /app
COPY ./requirements.txt /app/requirements.txt
RUN pip install -r /app/requirements.txt

COPY ./src /app/src

EXPOSE 8000

CMD ["fastapi", "run", "/app/src/main.py"]