FROM python:3.8
RUN mkdir /var/www
WORKDIR /var/www
COPY sample/requirements.txt .
RUN pip install -r requirements.txt
COPY sample/*.py ./sample/
COPY uwsgi.ini ./
CMD ["uwsgi", "--ini", "/var/www/uwsgi.ini"]
