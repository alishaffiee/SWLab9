FROM python:3.7-alpine

ENV PYTHONUNBUFFERED 1

RUN mkdir /code

WORKDIR /code

COPY . .

RUN pip install -r requirements.txt

EXPOSE 8001

COPY . .

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8001"]