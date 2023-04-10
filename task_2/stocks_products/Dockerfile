FROM python:3.9

COPY . ./app

WORKDIR app

RUN pip install --no-cache-dir --upgrade -r requirements.txt

EXPOSE 6060

RUN python manage.py migrate

CMD python manage.py runserver 0.0.0.0:6060