FROM python:3.6

WORKDIR /app
COPY requirements.txt uwsgi.ini ./

RUN pip install --no-cache-dir -r requirements.txt

COPY src/ ./

EXPOSE 3031
ENTRYPOINT ["/usr/local/bin/uwsgi", "--ini", "/app/uwsgi.ini", "--die-on-term"]